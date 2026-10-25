# 🔐 SecureCrypt

<div align="center">

# Secure File Protection & Management Platform

**A modern Django-based platform for secure file encryption, decryption, account protection, activity monitoring, and administrative management.**

<br>

![Django](https://img.shields.io/badge/Django-Backend-092E20?style=for-the-badge&logo=django)
![Python](https://img.shields.io/badge/Python-Application-3776AB?style=for-the-badge&logo=python)
![Security](https://img.shields.io/badge/Security-Focused-2E7D32?style=for-the-badge&logo=shield)
![Status](https://img.shields.io/badge/Status-Active-2563EB?style=for-the-badge)

<br>

> **SecureCrypt provides a clean and centralized environment for protecting files and monitoring security-related activity.**

</div>

---

## 📌 Overview

SecureCrypt is a secure file management platform designed to provide users with an organized environment for protecting and managing their files.

The application combines a modern dashboard experience with account management, encryption and decryption workflows, security activity monitoring, password management, notifications, and administrative controls.

The platform is divided into two major experiences:

- 👤 **User Portal** — Secure personal file operations and account management.
- 🛡️ **Administrator Portal** — User management, file monitoring, security logs, and platform insights.

---

# ✨ Key Features

<table>
<tr>
<td width="50%">

### 🔐 File Security
- Encrypt files through a dedicated workflow
- Decrypt protected files
- Centralized file management
- File activity visibility

</td>
<td width="50%">

### 👤 User Account System
- User registration
- Secure login
- Profile management
- Password management
- Account status monitoring

</td>
</tr>

<tr>
<td width="50%">

### 🛡️ Security Monitoring
- Security activity logs
- Login activity tracking
- Security event history
- Account protection status
- Event filtering interface

</td>
<td width="50%">

### 👨‍💼 Admin Management
- Registered user management
- User approval visibility
- Account status controls
- Administrative security logs
- File management dashboard

</td>
</tr>

<tr>
<td width="50%">

### 📊 Insights & Analytics
- User statistics
- Registration trends
- File statistics
- Top-user visibility
- Downloadable insights interface

</td>
<td width="50%">

### 🔔 Account Controls
- Notifications
- Settings
- Login security information
- Password and authentication controls
- Security preferences

</td>
</tr>
</table>

---

# 🖥️ Application Preview

## 🌙 User Dashboard

The main SecureCrypt dashboard provides users with an immediate overview of their account protection status, encrypted files, security events, and quick access to encryption and decryption actions.

<p align="center">
  <img src="screenshots/dashboard.png" alt="SecureCrypt User Dashboard" width="100%">
</p>

---

## 👥 User Management

The administrator can monitor registered users, account approval status, active users, pending accounts, rejected users, and account-level actions.

<p align="center">
  <img src="screenshots/user-management.png" alt="SecureCrypt User Management" width="100%">
</p>

---

## 🛡️ Security Logs

SecureCrypt provides a dedicated security log interface for reviewing recent account and security-related activity.

<p align="center">
  <img src="screenshots/security-logs.png" alt="SecureCrypt Security Logs" width="100%">
</p>

### Activity monitoring includes:

- Successful login events
- Security-related account activity
- Recent event history
- Event status indicators
- Time-based activity information

---

## ⚙️ Account Settings

Users can manage their account information and security preferences from a centralized settings interface.

<p align="center">
  <img src="screenshots/settings.png" alt="SecureCrypt Settings" width="100%">
</p>

---

## 📊 SecureCrypt Insights

The administration analytics section provides a high-level view of users, files, account statuses, and registration trends.

<p align="center">
  <img src="screenshots/insights.png" alt="SecureCrypt Insights Dashboard" width="100%">
</p>

---

## 📁 File Management

Administrators can monitor overall file statistics including total files, active files, and deleted files.

<p align="center">
  <img src="screenshots/file-management.png" alt="SecureCrypt File Management" width="100%">
</p>

---

# 🏗️ System Architecture

```text
                    ┌─────────────────────┐
                    │      SecureCrypt    │
                    │   Django Platform   │
                    └──────────┬──────────┘
                               │
              ┌────────────────┴────────────────┐
              │                                 │
      ┌───────▼────────┐               ┌────────▼────────┐
      │   User Portal   │               │  Admin Portal    │
      └───────┬────────┘               └────────┬────────┘
              │                                 │
     ┌────────┼─────────┐             ┌─────────┼──────────┐
     │        │         │             │         │          │
  Encrypt   Decrypt   Files        Users      Logs     Insights
     │        │         │             │         │          │
     └────────┴─────────┘             └─────────┴──────────┘
              │                                 │
              └──────────────┬──────────────────┘
                             │
                     ┌───────▼────────┐
                     │ Security Layer │
                     │ Authentication │
                     │ Activity Logs  │
                     │ Account Status │
                     └────────────────┘
```

---

# 🧩 Core Modules

| Module | Description |
|---|---|
| 🔐 Encrypt File | Interface for protecting user files |
| 🔓 Decrypt File | Interface for accessing protected files |
| 📁 My Files | Centralized user file management |
| 🔔 Notifications | Security and account notifications |
| 🛡️ Security Logs | User security activity history |
| 👤 Profile | User account information |
| ⚙️ Settings | Password and security preferences |
| 👥 User Management | Administrative account monitoring |
| 📊 Insights | Platform-level statistics and trends |
| 📁 File Management | Administrative file monitoring |
| 🔑 Password Management | Password change and reset workflows |

---

# 🎨 Interface Design

SecureCrypt follows two visual environments:

### User Interface
- Dark security-focused theme
- Blue accent system
- Sidebar navigation
- Status cards
- Quick action components
- Activity timeline design

### Administrator Interface
- Clean management dashboard
- Statistical cards
- Data tables
- Search and action controls
- Analytics visualization
- Centralized administration

---

# 🛠️ Technology Stack

| Technology | Usage |
|---|---|
| 🐍 Python | Core application language |
| 🎯 Django | Backend framework |
| 🌐 HTML5 | Page structure |
| 🎨 CSS3 | Interface styling |
| ⚡ JavaScript | Client-side interactions |
| 🗄️ Django ORM | Application data handling |
| 📊 Chart Visualization | Administrative insights |

---

# 📐 UML Diagrams

The following UML diagrams illustrate SecureCrypt's functional requirements, application structure, workflows, component organization, and deployment environment.

> **Note:** These are conceptual diagrams. Verify their actors, classes, attributes, and interactions against the actual implementation before using them as formal design documentation.

## 1. Use Case Diagram

The use case diagram represents the main interactions between users, administrators, and the external email service.

```mermaid
flowchart LR
    U["User"]
    A["Administrator"]
    E["Email Service"]

    subgraph SC["SecureCrypt System"]
        UC1(["Register and Login"])
        UC2(["Manage Profile"])
        UC3(["Encrypt File"])
        UC4(["Decrypt File"])
        UC5(["Manage Personal Files"])
        UC6(["Change or Reset Password"])
        UC7(["View Notifications"])
        UC8(["View Security Logs"])
        UC9(["Manage Users"])
        UC10(["Approve or Reject Accounts"])
        UC11(["Monitor Files"])
        UC12(["View Insights and Reports"])
        UC13(["Send Email Notifications"])
    end

    U --> UC1
    U --> UC2
    U --> UC3
    U --> UC4
    U --> UC5
    U --> UC6
    U --> UC7
    U --> UC8

    A --> UC8
    A --> UC9
    A --> UC10
    A --> UC11
    A --> UC12

    UC1 --> UC13
    UC6 --> UC13
    UC10 --> UC13
    UC13 --> E
```

## 2. Class Diagram

The class diagram describes the principal data entities and their conceptual relationships.

```mermaid
classDiagram
    class CustomUser {
        +username
        +email
        +phone
        +is_active
        +register()
        +authenticate()
        +manage_profile()
    }

    class EncryptedFile {
        +owner
        +original_filename
        +encrypted_file
        +encryption_method
        +expires_at
        +created_at
        +encrypt()
        +decrypt()
    }

    class SecurityLog {
        +user
        +event_type
        +description
        +timestamp
        +record_event()
    }

    class Notification {
        +user
        +message
        +is_read
        +created_at
        +mark_as_read()
    }

    class AdminActivityLog {
        +administrator
        +action
        +timestamp
        +record_action()
    }

    CustomUser "1" --> "0..*" EncryptedFile : owns
    CustomUser "1" --> "0..*" SecurityLog : generates
    CustomUser "1" --> "0..*" Notification : receives
    CustomUser "1" --> "0..*" AdminActivityLog : performs
```

## 3. Sequence Diagram

This sequence diagram illustrates a simplified login and file-encryption workflow.

```mermaid
sequenceDiagram
    actor User
    participant UI as Django Interface
    participant Auth as Authentication
    participant Enc as Encryption Service
    participant DB as Database
    participant Log as Security Logs

    User->>UI: Submit login credentials
    UI->>Auth: Validate credentials
    Auth->>DB: Retrieve account
    DB-->>Auth: Return account details

    alt Authentication successful
        Auth-->>UI: Login approved
        UI-->>User: Display dashboard
        User->>UI: Request file encryption
        UI->>Enc: Submit file and options
        Enc->>Enc: Validate and encrypt file
        Enc->>DB: Save file metadata
        Enc->>Log: Record security event
        UI-->>User: Return operation result
    else Authentication failed
        Auth->>Log: Record failed login
        Auth-->>UI: Reject login
        UI-->>User: Display error
    end
```

## 4. Activity Diagram

The activity diagram represents authentication, encryption, decryption, file validation, and security logging.

```mermaid
flowchart TD
    S([Start]) --> L[Enter Login Credentials]
    L --> V{Credentials Valid?}

    V -- No --> ER[Display Login Error]
    ER --> L

    V -- Yes --> H[Open Dashboard]
    H --> R{Select Operation}

    R -->|Encrypt| F[Select File]
    F --> FV{Request Valid?}
    FV -- No --> ERR[Display Validation Error]
    FV -- Yes --> ENC[Encrypt File]
    ENC --> SAVE[Save Encrypted File and Metadata]
    SAVE --> LOG[Record Security Event]

    R -->|Decrypt| D[Select Encrypted File]
    D --> P[Check Ownership, Permissions and Expiry]
    P --> AUTH{Authorized?}
    AUTH -- No --> DENY[Reject Request]
    AUTH -- Yes --> DEC[Decrypt and Verify File]
    DEC --> LOG

    R -->|Manage Files| M[View or Manage Files]
    M --> LOG

    LOG --> END([End])
    DENY --> END
    ERR --> END
```

## 5. Component Diagram

The component diagram illustrates the conceptual organization of the application.

```mermaid
flowchart TB
    B[Web Browser]

    subgraph APP["SecureCrypt Django Application"]
        UI[User Interface]
        AUTH[Authentication and Account Management]
        FILE[File Management]
        ENC[Encryption and Decryption]
        SEC[Security Monitoring]
        NOTIFY[Notification Service]
        REPORT[Insights and Reporting]
    end

    DB[(Application Database)]
    STORE[(File Storage)]
    EMAIL[External Email Service]

    B <--> UI
    UI --> AUTH
    UI --> FILE
    UI --> ENC
    UI --> SEC
    UI --> REPORT

    AUTH <--> DB
    FILE <--> DB
    ENC <--> DB
    ENC <--> STORE
    SEC --> DB
    NOTIFY <--> DB
    REPORT --> DB

    AUTH --> NOTIFY
    SEC --> NOTIFY
    NOTIFY --> EMAIL
```

## 6. Deployment Diagram

The deployment diagram represents the main runtime components and their connections.

```mermaid
flowchart TB
    USER["User or Administrator Browser"]

    subgraph HOST["Application Hosting Environment"]
        WEB["Gunicorn Web Server"]
        DJANGO["Django Application"]
        STATIC["Static Assets"]
    end

    DB[(Database)]
    STORAGE[(File Storage)]
    EMAIL["External Email Service"]

    USER <--> WEB
    WEB <--> DJANGO
    DJANGO --> STATIC
    DJANGO <--> DB
    DJANGO <--> STORAGE
    DJANGO <--> EMAIL
```

---

# 🔄 Data Flow Diagrams (DFD)

The following DFDs describe how data moves between external entities, application processes, and data stores.

## 1. Level 0 DFD — Context Diagram

The Level 0 DFD treats SecureCrypt as a single system and illustrates its interactions with the user, administrator, and email service.

```mermaid
flowchart LR
    U[User]
    A[Administrator]
    S((SecureCrypt System))
    E[Brevo Email Service]

    U -->|Registration, login and file requests| S
    S -->|Operation results and status| U

    A -->|Approval and management requests| S
    S -->|Dashboard information, logs and reports| A

    S -->|Email requests| E
    E -->|Email delivery status| S
```

## 2. Level 1 DFD — System Processes

The Level 1 DFD decomposes SecureCrypt into its main functional processes and associated data stores.

```mermaid
flowchart TD
    U[User]
    A[Administrator]
    E[Email Service]

    P1((1.0 Authentication and Account Approval))
    P2((2.0 File Encryption and Decryption))
    P3((3.0 File Management))
    P4((4.0 Security Monitoring))
    P5((5.0 Notifications and Reporting))

    D1[(D1 User Accounts)]
    D2[(D2 File Metadata)]
    D3[(D3 Security Logs)]
    D4[(D4 Notifications)]
    D5[(D5 Admin Activity Logs)]
    FS[(Encrypted File Storage)]

    U -->|Credentials and registration data| P1
    P1 <--> D1
    P1 -->|Authentication and account status| U

    A -->|Account approval decisions| P1
    P1 --> D1

    U -->|File and encryption requests| P2
    P2 <--> D1
    P2 <--> D2
    P2 <--> FS
    P2 -->|File operation result| U

    U -->|File management request| P3
    P3 <--> D2
    P3 <--> FS
    P3 -->|File status| U

    P1 -->|Authentication events| P4
    P2 -->|File operation events| P4
    P3 -->|File management events| P4
    P4 <--> D3
    P4 -->|Security alerts| P5

    P5 <--> D4
    P5 -->|Email requests| E
    P5 -->|Notifications and reports| U
    P5 -->|Administrative reports| A

    A -->|Administrative actions| P5
    P5 --> D5

    A -->|Security log request| P4
    P4 -->|Security event history| A
```

## 3. Level 2 DFD — Encryption and Decryption

The Level 2 DFD expands file-processing workflows into validation, encryption, storage, authorization, decryption, and logging steps.

```mermaid
flowchart TD
    U[User]

    subgraph ENC["Encryption Workflow"]
        E1((2.1 Receive File and Options))
        E2((2.2 Validate User and Request))
        E3((2.3 Encrypt File))
        E4((2.4 Store Encrypted File))
    end

    subgraph DEC["Decryption Workflow"]
        D1P((2.5 Validate File Access))
        D2P((2.6 Decrypt and Verify File))
    end

    ACC[(User Accounts)]
    META[(File Metadata)]
    LOG[(Security Logs)]
    STORE[(Encrypted File Storage)]

    U -->|File, password and expiry options| E1
    E1 --> E2

    E2 <--> ACC
    E2 -->|Valid request| E3
    E2 -->|Invalid request| DENY[Access Denied]

    E3 -->|Encrypted file data| E4
    E4 --> STORE
    E4 --> META
    E4 -->|Encryption result| U

    U -->|Decryption request and file reference| D1P
    D1P <--> ACC
    D1P <--> META

    D1P -->|Authorized request| D2P
    D1P -->|Unauthorized or expired| DENY

    STORE -->|Encrypted file data| D2P
    D2P -->|Successful decryption| U
    D2P -->|Invalid password or verification failure| DENY

    E2 -->|Validation event| LOG
    E4 -->|Encryption event| LOG
    D1P -->|Access decision| LOG
    D2P -->|Decryption event| LOG
    DENY -->|Rejected operation| LOG
```

---

# 🎨 Interface Design

SecureCrypt follows two visual environments:

### User Interface
- Dark security-focused theme
- Blue accent system
- Sidebar navigation
- Status cards
- Quick action components
- Activity timeline design

### Administrator Interface
- Clean management dashboard
- Statistical cards
- Data tables
- Search and action controls
- Analytics visualization
- Centralized administration

---

# 🛠️ Technology Stack

| Technology | Usage |
|---|---|
| 🐍 Python | Core application language |
| 🎯 Django | Backend framework |
| 🌐 HTML5 | Page structure |
| 🎨 CSS3 | Interface styling |
| ⚡ JavaScript | Client-side interactions |
| 🗄️ Django ORM | Application data handling |
| 📊 Chart Visualization | Administrative insights |

---

# 🚀 Getting Started

## 1. Clone the Repository

```bash
git clone https://github.com/Ramprakash-2008/SecureCrypt.git
cd SecureCrypt
```

## 2. Create a Virtual Environment

```bash
python -m venv venv
```

### Windows

```bash
venv\Scripts\activate
```

### Linux / macOS

```bash
source venv/bin/activate
```

## 3. Install Dependencies

```bash
pip install -r requirements.txt
```

## 4. Apply Database Migrations

```bash
python manage.py migrate
```

If you have changed your Django models and need new migrations, run:

```bash
python manage.py makemigrations
python manage.py migrate
```

## 5. Create an Administrator Account

```bash
python manage.py createsuperuser
```

## 6. Run the Application

```bash
python manage.py runserver
```

Open the local application:

```text
http://127.0.0.1:8000/
```

Django Administration:

```text
http://127.0.0.1:8000/admin/
```

---

# 📂 Suggested Project Structure

```text
SecureCrypt/
│
├── accounts/
│   ├── migrations/
│   ├── templates/
│   │   └── accounts/
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   └── views.py
│
├── securecrypt/
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
│
├── static/
│   ├── css/
│   ├── icons/
│   ├── images/
│   └── js/
│
├── media/
├── docs/
├── screenshots/
├── manage.py
├── requirements.txt
└── README.md
```

---

# 📸 Adding the Screenshots

For the README preview to work correctly on GitHub, create this structure and add your actual screenshots:

```text
screenshots/
├── dashboard.png
├── user-management.png
├── security-logs.png
├── settings.png
├── insights.png
└── file-management.png
```

The UML and DFD diagrams above use Mermaid code and therefore do not require separate image files.

---

# 🔒 Security-Oriented Design

SecureCrypt is designed around the idea that file protection should not feel complicated.

The interface emphasizes:

> **Visibility → Control → Protection → Monitoring**

Users can access security-related features from one centralized workspace, while administrators gain additional visibility into platform activity, user accounts, files, and security events.

---

# 🗺️ Future Improvements

- [ ] Two-factor authentication
- [ ] Advanced file sharing controls
- [ ] Email security alerts
- [ ] Device/session management
- [ ] File access expiration controls
- [ ] Advanced security analytics
- [ ] Role-based access control
- [ ] Improved audit reporting
- [ ] Cloud storage integration
- [ ] API support

---

# 🤝 Contributing

Contributions, improvements, and feature suggestions are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Make your changes.
4. Commit your changes.
5. Push to your branch.
6. Open a Pull Request.

---

# 📄 License

This project is intended for educational and development purposes.

---

<div align="center">

## 🔐 SecureCrypt

### Protect • Manage • Monitor

**A modern platform for secure file management and security monitoring.**

<br>

⭐ If you find this project useful, consider giving the repository a star.

</div>
