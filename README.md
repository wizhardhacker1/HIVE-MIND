<img width="50" height="50" alt="image" src="https://github.com/user-attachments/assets/d1333dc6-9464-4897-9c1b-46d23cd50450" /> Buy me a Coffee- buymeacoffee.com/wizhardhacker1

<p align="center">
  <img width="256" height="256" alt="HIVE MIND Logo" src="https://github.com/user-attachments/assets/46be5028-f919-43e1-a2b9-f06b05f3c939" />
</p>

<h1 align="center">HIVE MIND</h1>

<h3 align="center">Private. Local. Encrypted. Yours.</h3>

<p align="center">
  <strong>HIVE MIND 2.0.4 — FULL WINDOWS INSTALLER</strong>
</p>

<p align="center">
  <img width="1919" height="730" alt="HIVE MIND Banner" src="https://github.com/user-attachments/assets/54926fb8-75bd-4c37-a784-b0b8e5fb960d" />
</p>

---

## 🐝 What is HIVE MIND?

**HIVE MIND** is a local-first knowledge vault and AI chat platform for Windows.

It is designed to ingest, organize, encrypt, search, and discuss your own files while keeping the core knowledge base and AI workflow on your machine.

> **YOUR FILES → YOUR VAULT → YOUR AI → YOUR KNOWLEDGE**

HIVE MIND combines encrypted document storage, intelligent ingestion, vault-specific AI conversations, local LLM processing, OCR, legacy document support, access controls, auditing, and backups into one desktop knowledge system.

---

## 🖥️ HIVE MIND Interface


The HIVE MIND interface provides centralized access to:

* Knowledge vaults
* Document ingestion
* Local AI conversations
* Search
* Vault settings
* System status
* User administration
* Security controls
* Backup management

---

## 🧠 How HIVE MIND Works

```text
FILES
  │
  ▼
INGEST
  │
  ▼
EXTRACT
  │
  ▼
ENCRYPT
  │
  ▼
INDEX
  │
  ▼
VAULT
  │
  ▼
LOCAL AI
  │
  ▼
SEARCH + CHAT
  │
  ▼
KNOWLEDGE
```

Your documents become a private, searchable knowledge base that you can interact with using a locally provisioned AI model.

---

## 🗄️ Knowledge Vaults

HIVE MIND organizes information into independent **Vaults**.

Each vault can maintain its own:

* Documents
* Searchable knowledge
* Ingestion configuration
* Chat history
* AI context
* Permissions
* Processing settings

This allows completely different knowledge collections to coexist without mixing their conversations or document context.

```text
HIVE MIND
│
├── VAULT A
│   ├── Documents
│   ├── Index
│   ├── Settings
│   └── Chat
│
├── VAULT B
│   ├── Documents
│   ├── Index
│   ├── Settings
│   └── Chat
│
└── VAULT C
    ├── Documents
    ├── Index
    ├── Settings
    └── Chat
```

---

## 💬 Per-User / Per-Vault AI Chat

Every vault has its own encrypted chat environment.

The AI uses information ingested into the selected vault to provide answers grounded in that vault's knowledge instead of mixing information from unrelated collections.

```text
USER
  │
  ▼
VAULT
  │
  ▼
ENCRYPTED CHAT
  │
  ▼
VAULT KNOWLEDGE
```

Chat data is separated by both **user and vault**.

---

## 🦙 Local AI — Meta Llama 3.2 3B

HIVE MIND provisions **Meta Llama 3.2 3B** for local/offline AI chat.

The model is served locally using an **Ollama loopback-only service**.

```text
HIVE MIND
     │
     ▼
LOCAL OLLAMA
     │
     ▼
LLAMA 3.2 3B
     │
     ▼
VAULT CONTEXT
     │
     ▼
LOCAL RESPONSE
```

The local Ollama service is bound to the local machine rather than intentionally exposed as a network AI endpoint.

Once the required model components are provisioned, normal local vault conversations do not require a cloud LLM.

---

## 🔐 Encryption

HIVE MIND is designed around encrypted storage rather than treating encryption as an optional add-on.

Large files can be handled using **streaming encryption**, avoiding the need to load an entire multi-gigabyte file into memory before encrypting it.

### Security capabilities

* Encrypted vault data
* Encrypted chat
* Per-user separation
* Per-vault separation
* Streaming file encryption
* Secure persistent storage
* Role-based access control
* Audit logging
* Backup support

---

## 📁 Document Ingestion

HIVE MIND is designed to work with the types of files commonly found in real-world knowledge repositories.

Processing capabilities include:

* Modern Microsoft Office documents
* Legacy Office extraction
* PDF documents
* Text documents
* Email content
* PST archives
* MSG messages
* Images
* OCR processing hooks
* Large files
* Streamed uploads

Each vault can maintain its own ingestion settings.

---

## 📦 Up to 20 GB Streamed Uploads

HIVE MIND supports streamed uploads of up to:

# **20 GB**

Instead of loading the entire file into application memory, large files can move through the processing pipeline as a stream.

```text
LARGE FILE
    │
    ▼
  STREAM
    │
    ├──► PROCESS
    │
    ├──► ENCRYPT
    │
    └──► STORE
```

This architecture is designed to support substantially larger files than conventional small-document upload systems.

---

## 📧 PST & MSG Processing

HIVE MIND includes processing support for email-based knowledge sources.

### Microsoft Outlook PST

PST archives can be incorporated into the ingestion pipeline, allowing archived email information to become part of a vault's searchable knowledge.

### Microsoft Outlook MSG

Individual MSG email files can also be processed by the ingestion system.

This allows historical communications to become part of the knowledge base where supported by the configured extraction pipeline.

---

## 👁️ OCR

HIVE MIND includes OCR integration hooks for extracting searchable information from image-based content.

Useful sources include:

* Scanned documents
* Image-based PDFs
* Screenshots
* Forms
* Archived records
* Photographed documents

OCR behavior can be configured through the ingestion system.

---

## 🏢 Legacy Microsoft Office Support

Real-world archives often contain documents created before modern DOCX and XLSX formats.

HIVE MIND includes **legacy Microsoft Office extraction support** as part of its ingestion architecture.

The objective is to make older organizational knowledge searchable without requiring every document to be manually converted first.

---

## 👥 Role-Based Access Control

HIVE MIND includes **RBAC — Role-Based Access Control**.

```text
USER
 │
 ▼
ROLE
 │
 ▼
PERMISSIONS
 │
 ├──► Vault Access
 ├──► Document Access
 ├──► Administration
 └──► System Functions
```

RBAC provides the foundation for controlling which users can access or administer different areas of HIVE MIND.

---

## 📋 Audit Logging

Security-sensitive operations can be recorded through the HIVE MIND audit logging system.

Audit records provide a history that can help administrators understand:

* User activity
* Vault activity
* Administrative actions
* Security-relevant events
* System changes

---

## 💾 Backups

HIVE MIND separates the application from persistent user data.

```text
HiveMind
│
├── app
│   └── Application Files
│
└── data
    └── Persistent HIVE MIND Data
```

This separation is designed to make application upgrades safer and reduce the chance of persistent data being replaced during an update.

---

## 🔄 Hive Memory Migration

HIVE MIND can automatically migrate data from an existing **Hive Memory** installation.

Migration occurs when:

```text
Existing Hive Memory Data
           +
HIVE MIND Has No Database
           │
           ▼
   AUTOMATIC MIGRATION
           │
           ▼
       HIVE MIND
```

This provides an upgrade path from the earlier Hive Memory application to HIVE MIND.

---

# 🪟 Windows Installation

## HIVE MIND 2.0.4 FULL WINDOWS INSTALLER

### 1. Extract the ZIP

Extract the complete HIVE MIND distribution before running the installer.

> **Do not run the installer directly from inside the ZIP archive.**

### 2. Run the Installer

Double-click:

```bat
INSTALL_HIVE_MIND.bat
```

### 3. Existing Data Migration

If an existing Hive Memory installation is detected and HIVE MIND does not yet contain a database, existing data is automatically migrated.

### 4. Application Installation

Application files are installed under:

```text
%LOCALAPPDATA%\HiveMind\app
```

Persistent HIVE MIND data is stored separately under:

```text
%LOCALAPPDATA%\HiveMind\data
```

### 5. Local AI Provisioning

The installer provisions the components required for local AI chat using:

**Meta Llama 3.2 3B + Ollama**

Ollama is configured for local/loopback access by HIVE MIND.

---

## 📂 Windows Directory Structure

```text
%LOCALAPPDATA%
│
└── HiveMind
    │
    ├── app
    │   └── HIVE MIND Application
    │
    └── data
        ├── Database
        ├── Vault Data
        ├── Encrypted Files
        ├── Chat Data
        ├── Indexes
        ├── Logs
        └── Backups
```

Application files and persistent data are deliberately separated.

---

# ⚙️ Core Features

| Feature                     | HIVE MIND |
| --------------------------- | :-------: |
| 🦙 Meta Llama 3.2 3B        |     ✅     |
| 🧠 Local AI Chat            |     ✅     |
| 🔌 Ollama Integration       |     ✅     |
| 📴 Offline-Capable Chat     |     ✅     |
| 🗄️ Multiple Vaults         |     ✅     |
| 💬 Vault-Specific Chat      |     ✅     |
| 👤 Per-User Chat            |     ✅     |
| 🔐 Encrypted Chat           |     ✅     |
| 🔒 Encrypted Storage        |     ✅     |
| 🌊 Streaming Encryption     |     ✅     |
| 📦 20 GB Streamed Uploads   |     ✅     |
| ⚙️ Vault-Specific Ingestion |     ✅     |
| 📧 PST Processing           |     ✅     |
| ✉️ MSG Processing           |     ✅     |
| 👁️ OCR Hooks               |     ✅     |
| 📄 Legacy Office Extraction |     ✅     |
| 👥 RBAC                     |     ✅     |
| 📋 Audit Logging            |     ✅     |
| 💾 Backups                  |     ✅     |
| 🔄 Hive Memory Migration    |     ✅     |
| 🪟 Windows Installer        |     ✅     |

---

# 🛡️ Local-First Architecture

HIVE MIND is built around a fundamental principle:

> ### **Your knowledge should remain under your control.**

Instead of making cloud AI the center of the architecture, HIVE MIND places the **Vault** at the center.

```text
                 ┌─────────────┐
                 │  HIVE MIND  │
                 └──────┬──────┘
                        │
          ┌─────────────┼─────────────┐
          │             │             │
          ▼             ▼             ▼
       VAULTS       SECURITY       LOCAL AI
          │             │             │
          ▼             ▼             ▼
      DOCUMENTS     ENCRYPTION    LLAMA 3.2 3B
          │             │             │
          └─────────────┼─────────────┘
                        │
                        ▼
                 PRIVATE KNOWLEDGE
```

---

# 🔁 The HIVE MIND Workflow

```text
COLLECT
   ↓
INGEST
   ↓
EXTRACT
   ↓
ENCRYPT
   ↓
INDEX
   ↓
SEARCH
   ↓
CHAT
   ↓
DISCOVER
   ↓
KNOWLEDGE
```

HIVE MIND isn't designed simply to store documents.

It is designed to turn a private collection of files into **usable, searchable knowledge**.

---

# 🚧 Project Status

## HIVE MIND 2.0.4

HIVE MIND is under active development.

Document processors, AI models, indexing systems, security controls, user interfaces, installation behavior, and other components may change as the platform evolves.

> **Back up important data before installing development releases or performing major upgrades.**

---

# ⚠️ Security Notice

HIVE MIND includes encryption and local-processing features intended to improve the privacy of stored information.

No software system should be assumed to provide absolute security.

Users deploying HIVE MIND with confidential, regulated, proprietary, or otherwise sensitive information should independently evaluate the application's security controls and configuration for their environment.

---

<p align="center">
  <img width="256" height="256" alt="HIVE MIND Logo" src="https://github.com/user-attachments/assets/46be5028-f919-43e1-a2b9-f06b05f3c939" />
</p>

<h1 align="center">🐝 HIVE MIND</h1>

<h3 align="center">Your Files. Your Vault. Your AI.</h3>

<p align="center">
  <strong>FILES → INGEST → ENCRYPT → INDEX → CHAT → KNOWLEDGE</strong>
</p>

<p align="center">
  <strong>HIVE MIND 2.0.4</strong>
</p>

<p align="center">
  <strong>Private. Local. Encrypted. Yours.</strong>
</p>
