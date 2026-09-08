HIVE MIND

### Private. Local. Encrypted. Yours.

**HIVE MIND 2.0.4 — FULL WINDOWS INSTALLER**

HIVE MIND is a local-first knowledge vault and AI chat platform for Windows.

It is designed to ingest, organize, encrypt, search, and discuss your own files while keeping the core knowledge base and AI workflow on your machine.

The idea is simple:

> **YOUR FILES → YOUR VAULT → YOUR AI → YOUR KNOWLEDGE**

HIVE MIND combines encrypted document storage, intelligent ingestion, vault-specific AI conversations, local LLM processing, OCR, legacy document support, access controls, auditing, and backups into one desktop knowledge system.

---

# 🧠 What Is HIVE MIND?

Traditional AI systems often require sending information to external services.

HIVE MIND is designed around a different model:

```text
FILES
  │
  ▼
INGEST
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

# 🖼️ HIVE MIND Interface

<!-- Replace this section with your first GitHub screenshot -->

<!--
<img width="1700" alt="HIVE MIND Dashboard" src="YOUR_GITHUB_IMAGE_URL" />
-->

The main HIVE MIND interface provides access to your vaults, document ingestion, local AI conversations, search, system status, and administration.

---

# 🗄️ Knowledge Vaults

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

# 💬 Per-Vault AI Chat

Every vault has its own encrypted chat environment.

The AI can use information ingested into that vault to provide answers grounded in the vault's knowledge instead of mixing information from unrelated collections.

Chat data is separated by both:

```text
USER
  │
  └── VAULT
       │
       └── ENCRYPTED CHAT
```

This provides **per-user / per-vault encrypted conversations**.

---

# 🦙 Local AI — Meta Llama 3.2 3B

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

The local service is intentionally bound to the local machine rather than exposed as a network AI endpoint.

Once the required model components have been provisioned, the local chat architecture is designed to operate without requiring a cloud LLM for normal vault conversations.

---

# 🔐 Encryption

HIVE MIND is designed around encrypted storage rather than treating encryption as an optional add-on.

Large files can be processed using **streaming encryption**, avoiding the need to load an entire multi-gigabyte file into memory before encrypting it.

The platform includes support for:

* Encrypted vault data
* Encrypted chat
* Per-user separation
* Per-vault separation
* Streaming file encryption
* Secure persistent storage
* Access controls
* Audit logging

---

# 📁 Document Ingestion

HIVE MIND is designed to ingest many of the file formats commonly found in real-world knowledge repositories.

Supported processing capabilities include:

* Modern Office documents
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

Vault-specific ingestion settings allow different vaults to use different processing behavior.

---

# 📦 Large File Support

HIVE MIND supports streamed uploads of up to:

## **20 GB**

Large files are streamed rather than requiring the entire file to be held in application memory.

The same architecture is used for large-file encryption.

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

This makes HIVE MIND suitable for substantially larger knowledge collections than systems designed only around small document uploads.

---

# 📧 Email & Archive Processing

HIVE MIND includes processing support for email-based knowledge sources, including:

### PST

Microsoft Outlook PST archives can be incorporated into the ingestion pipeline.

### MSG

Individual Outlook message files can also be processed.

This allows archived communications to become part of a searchable knowledge vault where supported by the configured extraction pipeline.

---

# 👁️ OCR

HIVE MIND includes OCR integration hooks for extracting searchable information from image-based content.

This is useful for content such as:

* Scanned documents
* Image-based PDFs
* Screenshots
* Forms
* Archived records
* Photographed documents

OCR behavior can be controlled as part of the ingestion configuration.

---

# 🏢 Legacy Office Documents

Real-world archives frequently contain documents created long before modern DOCX and XLSX formats.

HIVE MIND therefore includes **legacy Microsoft Office extraction support** as part of its document-processing architecture.

The goal is to make old organizational knowledge searchable rather than requiring every document to be manually converted first.

---

# 👥 Role-Based Access Control

HIVE MIND includes **RBAC — Role-Based Access Control**.

RBAC provides a foundation for controlling what different users are permitted to access or manage.

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

---

# 📋 Audit Logging

Security-sensitive operations can be recorded through HIVE MIND's audit logging system.

Audit logs provide a history that can help administrators understand activity within the application and investigate changes or access events.

---

# 💾 Backups

HIVE MIND includes backup capabilities for protecting persistent application data.

The application architecture deliberately separates the program itself from persistent data.

```text
HiveMind
│
├── app
│   └── Application Files
│
└── data
    └── Persistent HIVE MIND Data
```

This separation helps prevent application upgrades from unnecessarily replacing user data.

---

# 🔄 Hive Memory Migration

HIVE MIND can automatically migrate data from an existing **Hive Memory** installation.

Migration occurs when:

```text
Existing Hive Memory Data
           +
HIVE MIND Has No Existing Database
           │
           ▼
   AUTOMATIC MIGRATION
           │
           ▼
       HIVE MIND
```

This allows users of the previous Hive Memory application to transition to HIVE MIND without intentionally starting with an empty knowledge base.

---

# 🪟 Windows Installation

## HIVE MIND 2.0.4 FULL WINDOWS INSTALLER

### 1. Extract the ZIP

Extract the complete HIVE MIND distribution before running the installer.

Do **not** run the installer directly from inside the ZIP archive.

### 2. Run the Installer

Double-click:

```bat
INSTALL_HIVE_MIND.bat
```

### 3. Existing Data Migration

If an existing Hive Memory installation is detected and HIVE MIND does not yet contain a database, the installer automatically migrates the existing data.

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

The Ollama service is configured for loopback/local access by HIVE MIND.

---

# 📂 Windows Directory Structure

A typical installation follows this structure:

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

Separating application and persistent data makes upgrading HIVE MIND safer and easier.

---

# ⚙️ Core Features

| Feature                  | HIVE MIND |
| ------------------------ | --------- |
| Local AI Chat            | ✅         |
| Meta Llama 3.2 3B        | ✅         |
| Ollama Integration       | ✅         |
| Offline-Capable Chat     | ✅         |
| Multiple Vaults          | ✅         |
| Vault-Specific Chat      | ✅         |
| Per-User Chat            | ✅         |
| Encrypted Chat           | ✅         |
| Encrypted Storage        | ✅         |
| Streaming Encryption     | ✅         |
| 20 GB Streamed Uploads   | ✅         |
| Vault-Specific Ingestion | ✅         |
| PST Processing           | ✅         |
| MSG Processing           | ✅         |
| OCR Hooks                | ✅         |
| Legacy Office Extraction | ✅         |
| RBAC                     | ✅         |
| Audit Logging            | ✅         |
| Backups                  | ✅         |
| Hive Memory Migration    | ✅         |
| Windows Installer        | ✅         |

---

# 🛡️ Local-First Architecture

HIVE MIND is built around a fundamental principle:

> **Your knowledge should remain under your control.**

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

The objective isn't simply to store documents.

The objective is to make a private collection of information **usable as knowledge**.

---

# 🚧 Project Status

## HIVE MIND 2.0.4

HIVE MIND is under active development.

Document processors, AI models, indexing systems, security controls, user interfaces, installation behavior, and other components may continue to change as the platform evolves.

Back up important data before installing development releases or performing major upgrades.

---

# ⚠️ Security Notice

HIVE MIND includes encryption and local-processing features intended to improve the privacy of stored information.

No software system should be assumed to provide absolute security.

Users deploying HIVE MIND with confidential, regulated, proprietary, or otherwise sensitive information should independently evaluate the application's security controls and configuration for their environment.

---

# 🐝 HIVE MIND

### Your Files. Your Vault. Your AI.

```text
FILES → INGEST → ENCRYPT → INDEX → CHAT → KNOWLEDGE
```

**HIVE MIND 2.0.4**

**Private. Local. Encrypted. Yours.**

<img width="1442" height="824" alt="image" src="https://github.com/user-attachments/assets/4222517b-3ce8-4c7b-9854-54fd77cd5b56" />

