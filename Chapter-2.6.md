## 2.6. Tactical-Level Domain-Driven Design

### 2.6.1. Bounded Context: Identity and Access Management (IAM)

Este contexto delimitado es de alcance global y puramente técnico. Su única responsabilidad es gestionar la identidad de los usuarios registrados en Splitly, emitir tokens de acceso y validar las credenciales. No contiene lógica de negocio sobre las casas o la distribución de pagos; únicamente proporciona una identidad segura (UUID/ID) que los demás contextos (como Household Management) utilizarán para vincular sus propias entidades.

#### 2.6.1.1. Domain Layer

**Entidades Principales**

**User (Aggregate Root)**
* **Propósito:** Representa la identidad global del usuario dentro de la plataforma Splitly.
* **Atributos principales:**
    * `id` — Identificador único global (UUID), utilizado como clave foránea conceptual en otros contextos.
    * `email` — Correo electrónico único (usado como credencial principal de login).
    * `passwordHash` — Hash seguro de la contraseña.
    * `firstName`, `lastName` — Datos básicos de perfil.
    * `isActive` — Estado de la cuenta en el sistema.
    * `systemRoles` — Lista de roles del sistema (ej. `USER`, `SYS_ADMIN`). *Nota: Los roles de administración del hogar se manejan en Household Management.*
* **Métodos principales:**
    * `updateCredentials(email, newPasswordHash)`
    * `lockAccount()`, `unlockAccount()`

**Role (Entity)**
* **Propósito:** Define niveles de acceso al sistema (a nivel de la plataforma general, no de la casa).
* **Atributos principales:**
    * `id`
    * `name` — (ej. `STANDARD_USER`, `SUPPORT_ADMIN`)

**Value Objects**
* **EmailAddress:** Reglas de validación de formato (Regex).
* **EncryptedPassword:** Encapsula el proceso de hashing (BCrypt/Argon2) y validación de fuerza.
* **AuthToken:** Representa el JWT emitido, encapsulando sus claims (ID del usuario, expiración).

**Domain Services**
* **AuthenticationService:** Coordina la validación de credenciales (email + password) contra la base de datos y solicita la emisión del token.
* **TokenGeneratorService:** Construye y firma digitalmente el Access Token y Refresh Token.

**Commands (CQRS)**
* `RegisterAccountCommand`
* `AuthenticateUserCommand`
* `ResetPasswordCommand`

**Queries (CQRS)**
* `ValidateTokenQuery`
* `GetBasicProfileQuery`

**Events**
* `AccountRegisteredEvent` (Notifica a otros contextos que un nuevo usuario global existe. Por ejemplo, `Household Management` podría escuchar esto para preparar un perfil vacío).