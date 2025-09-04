# API Documentation Questions for Tech Writers

## 1. General API Understanding
- What kind of API is this? (REST, GraphQL, gRPC, hybrid)
- Is there a base URL and versioning scheme? (e.g., `/api/v1/...`)
- How is authentication handled? (API keys, OAuth2, JWT, RBAC tokens)
- What data formats are supported? (JSON, XML, CSV, multipart)
- What error codes and conventions are used? (Standard HTTP vs. custom codes)

## 2. Resource Model & Structure
- What are the primary resources? (Applications, Models, Functions, Storage, Databases, Vectors)
- How are resources identified? (UUIDs, human-readable names, or both)
- What is the lifecycle of each resource? (create, read, update, delete, configure, deploy)
- Are relationships between resources defined? (e.g., Applications → Models → Storage)

## 3. Endpoints & Operations
- What are the CRUD endpoints for each resource?
- Are there batch or bulk operations?
- Are there asynchronous operations? (e.g., training a model, provisioning storage)
- How do we poll or check job status?

## 4. Usage & Integration
- Do client SDKs exist? (Python, JavaScript, Java, others)
- Is code generation possible via an OpenAPI/Swagger spec?
- Are there rate limits, quotas, or pagination rules?
- Can resources be swapped seamlessly (e.g., S3 → Azure Blob via UUID abstraction)?

## 5. Security & Governance
- How is access scoped? (project-level, org-level, per-user)
- What metadata/logs are exposed via API?
- Is RBAC configurable via API?
- How are sensitive models/data hosted? (cloud vs. local)

## 6. Developer Experience
- Are there sandbox or test environments?
- Do APIs return helpful error messages?
- Are example requests/responses provided in docs?
- Are common use cases documented? (end-to-end workflows)

