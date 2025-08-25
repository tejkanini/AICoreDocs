# AI Core: SME-Specific Leading Q & A

This document provides structured, leading questions for different SME groups (Developers, QA, Business Analysts, Product Leads).  
The goal is to build understanding progressively, from high-level workflows down to detailed technical and governance considerations.  

---

## Developer-Focused Questions

1. Walk me through the **end-to-end workflow of creating an application** in AI Core from pre-creation, creation, to publishing.  
2. At which stage are **building blocks** (storage, databases, vector DBs, models, functions) introduced into the workflow?  
3. Are these five building blocks **fixed components**, or can developers add new types?  
4. How do **connectors** fit into this workflow, do they automatically link blocks, or must developers configure them manually?  
5. When connectors are configured, how is the **interaction between blocks abstracted** (e.g., via UUIDs)?  
6. If a developer swaps one provider for another (e.g., S3 Azure Blob), what exactly changes in the code or app?  
7. For pro-code workflows, what languages and frameworks are officially supported?  
8. Can no-code apps created by business users be **exported into code** and extended by developers?  
9. How does AI Core handle **versioning** of applications and building blocks?  
10. Once an application is created, what does the **publishing process** look like who can publish, where does it go, and how is it consumed?  

---

## QA-Focused Questions

1. Is there a **sandbox or staging mode** where apps can be tested before publishing?  
2. What kinds of **automated tests** (unit, integration, regression) are in place for building blocks and connectors?  
3. How are **runtime errors** (e.g., failed model calls, missing storage, connector failure) surfaced to the user or admin?  
4. Can applications **retry failed operations** or recover gracefully without manual intervention?  
5. How does QA verify **RBAC configurations** to ensure no unauthorized access to data/models?  
6. What benchmarks or metrics exist to measure **performance under load** (e.g., large datasets in vector DBs, high concurrency on model calls)?  
7. Are there any known **scalability limits** (e.g., max apps per tenant, max connectors per app)?  

---

## Business Analyst Questions

1. Can you confirm the **primary personas** (developer, data scientist, business user) the platform is designed for?  
2. For each persona, what are the **expected workflows** (e.g., a business user creating a no-code app, a developer extending it)?  
3. How much **overlap** is expected between personas (e.g., can a business user hand over a draft app to a developer for refinement)?  
4. What are the **most common business scenarios** targeted today (e.g., customer support chatbots, data dashboards, document classification)?  
5. Are there **industry-specific templates** available (finance, healthcare, retail), or are these on the roadmap?  
6. How does AI Core integrate into **existing enterprise systems** (ERP, CRM, data warehouses)?  
7. What KPIs or adoption metrics will define whether a deployment of AI Core is **successful** for a business unit?  

---

## Product Led Questions

1. What **unique problem** does AI Core solve that other AI platforms do not?  
2. Is the platform primarily intended for **internal enablement** or as a **commercial offering** for customers?  
3. How do we plan to address **vendor lock-in concerns**, especially around models and storage providers?  
4. What is the **product roadmap** for introducing new templates, block types, or connectors?  
5. Will AI Core support **multi-tenancy** for large enterprises with multiple business units?  
6. Is there a roadmap for **offline or on-prem deployment** for regulated industries?  
7. What are the **security and compliance guarantees** (RBAC granularity, logging, data residency)?  
8. How do we envision **scaling adoption**:  internal marketplace, subscription model, or open sharing?  

