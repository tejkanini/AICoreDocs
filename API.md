# AI Core API Reference

## 1. Getting Started
- Base URL
- API Versioning
- Supported Data Formats
- Rate Limits & Quotas

## 2. Authentication
- API Keys
- OAuth2 / JWT Tokens
- Role-Based Access Control (RBAC)
- Example Authentication Flows

## 3. Error Handling
- Standard HTTP Status Codes
- AI Core-Specific Error Codes
- Error Response Format
- Retry & Timeout Guidelines

---

## 4. Core Resources

### 4.1 Applications
- **Endpoints**
  - `POST /applications` — Create an application
  - `GET /applications` — List applications
  - `GET /applications/{id}` — Retrieve application details
  - `PUT /applications/{id}` — Update application
  - `DELETE /applications/{id}` — Delete application
- **Sub-resources**
  - Application Templates
  - Application Deployment
  - Application Logs
- **Examples**
  - Request/Response payloads
  - Code snippets (Python, JavaScript, Java)

### 4.2 Storage
- Supported Types: S3, Azure Blob, Dropbox
- Endpoints
  - `POST /storage`
  - `GET /storage`
  - `GET /storage/{id}`
  - `DELETE /storage/{id}`
- Usage with UUID abstraction
- Example code snippets (multi-language)

### 4.3 Databases
- Supported Types: SQL, NoSQL, CSV, SQLite
- Endpoints
  - CRUD operations for databases
  - Query execution (`POST /databases/{id}/query`)
- Example: Insert/Update/Delete

### 4.4 Vector Databases
- Supported Providers (Pinecone, file-based, etc.)
- Endpoints
  - `POST /vectors`
  - `POST /vectors/{id}/search`
- Example: Semantic search API

### 4.5 Models
- Supported Types: OpenAI, Azure, Bedrock, Local
- Endpoints
  - `POST /models`
  - `POST /models/{id}/invoke`
  - `POST /models/{id}/train` (if applicable)
- Example: Chat completion, embeddings, classification

### 4.6 Functions
- Built-in Functions (text-to-speech, OCR, etc.)
- Endpoints
  - `POST /functions`
  - `POST /functions/{id}/execute`
- Example: Speech-to-text request

---

## 5. Workflow APIs
- Linking Resources (Apps → Models → Storage)
- Agent Builder APIs (prompt-driven app creation)
- No-code/Low-code Workflow Endpoints

---

## 6. Security & Governance APIs
- User Management
- Roles & Permissions
- Audit Logs
- Metering & Usage APIs

---

## 7. SDKs & Integration
- Python SDK
- JavaScript SDK
- Java SDK
- Example integrations

---

## 8. Appendix
- Glossary
- Changelog
- Deprecation Policy

