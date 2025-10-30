# Architectural Standard: Vendor-Supplied APIs

This standard outlines the minimum expectations and architectural principles for integrating vendor-supplied (off-the-shelf) Application Programming Interfaces (APIs) into enterprise systems. It draws upon UK Government guidance, OpenAPI specifications, ISO standards, and global best practices.

This standard ensures that vendor-supplied APIs are secure, interoperable, and maintainable, supporting enterprise architecture goals and reducing integration risk.

## Scope and Applicability

This standard applies to all externally sourced APIs used within the enterprise, including:

- Commercial APIs provided by vendors
- Open APIs from public sector or community sources
- APIs embedded within SaaS platforms

> **Note:** This standard does **not** apply to APIs developed in-house or from first principles, as those require more direct responsibility for design, documentation, security, lifecycle, and operational readiness.

## Design Principles

Vendor APIs must adhere to the following design principles:

- **Contract-first:** APIs must be described using OpenAPI 3.1+ or equivalent.
- **RESTful or justified alternative:** REST is preferred; GraphQL/gRPC acceptable with rationale.
- **Composable and reusable:** APIs should support modular integration.
- **Predictable structure:** Consistent naming, versioning, and error handling.

## Security Requirements

Vendor APIs must meet enterprise security standards:

- **Authentication:** OAuth 2.0, OpenID Connect, or mutual TLS.
- **Transport Security:** HTTPS with TLS 1.2+.
- **Data Protection:** Encryption in transit and at rest.
- **Rate Limiting:** Must prevent abuse and support throttling.
- **Audit Logging:** Usage must be traceable.

## Governance and Lifecycle

Vendors must demonstrate:

- **OpenAPI Specification:** Complete and valid documentation.
- **Versioning Strategy:** Clear versioning and deprecation policy.
- **Change Management:** Release notes and impact assessments.
- **Support Channels:** Escalation paths and SLAs.
- **Sandbox Environment:** For integration testing.

## Integration and Interoperability

Vendor APIs must:

- Use standard protocols (REST, GraphQL, gRPC)
- Provide consistent response formats
- Include health check endpoints
- Support catch-retry and timeout logic

### Additional Requirements for Webhooks

Vendor APIs that support webhooks must also provide:

- Secure webhook registration and authentication (e.g., secret tokens, IP whitelisting)
- Example webhook payloads and explicit metadata
- Documentation of event types, retry logic, and failure handling
- Privacy controls for webhook data transmission

## Compliance and Assurance

Vendor APIs must align with:

- **ISO/IEC 27001:** Information security
- **ISO/IEC 25010:** Software quality
- **OpenAPI 3.1+** or equivalent

Specific use cases may require additional compliance with:

- UK Government Technology Code of Practice
- Data Protection Impact Assessments (DPIAs)
- Memoranda of Understanding (MOUs) for sensitive data

Vendors must attest to:

- Secure development practices
- Penetration testing and static code analysis

## Privacy by Design

Vendor APIs must follow privacy-first principles:

- **Minimal Data Exposure:** Only expose data fields required for the consuming service.
- **Scoped Access:** Use authentication scopes to limit access to necessary endpoints.
- **Purpose Binding:** Data must be used only for its documented and intended purpose.
- **Field-Level Filtering:** Support selective field queries to avoid over-fetching.
- **PII Protection:** Personally identifiable information (PII) must be redacted, anonymised, or excluded unless explicitly required and justified.

### Example Payloads and Explicit Metadata

Vendors must provide example request and response payloads, and explicit metadata (e.g., field descriptions, data types, privacy classification) in their API documentation and specifications. This supports privacy by design, enabling governance teams to assess data minimisation and compliance with privacy requirements.

## Procurement Considerations

Contracts must include:

- API availability guarantees
- Support for OpenAPI or equivalent
- Security and data handling clauses
- Exit strategy and data portability

### Cost Model Transparency

Contracts must specify the following items, recognising that some APIs are pay-as-you-go or use metering as part of their cost model:

- Pricing structure (e.g., per call, per data volume, per user)
- Metering and reporting mechanisms
- Thresholds for usage alerts and cost controls
- Terms for scaling, overage charges, and billing cycles

---

## Alignment with Architecture Principles

This standard is designed to fully align with the following [architecture principles](https://github.com/buildbod/Architecture/blob/main/Templates/Principles/README.md):

### From Core Architecture Principles

- **Primacy of Principles:** Ensures consistent, group-wide API evaluation and integration, supporting compliance and risk management.
- **Maximise Benefits:** Assesses APIs for enterprise-wide value, not just local fit.
- **Design for Resilience:** Requires SLAs, redundancy, and recovery plans for business continuity.
- **Comply with Regulations:** Ensures APIs meet legal, regulatory, and internal policy requirements.
- **Enterprise Data as an Asset:** Privacy by Design and data protection requirements ensure APIs treat data as a managed, valuable asset.
- **Ease-of-Use:** Mandates well-documented, easy-to-integrate APIs for user experience and productivity.
- **Requirements-Based Change:** API adoption is driven by documented business needs and subject to architecture checks.
- **Control Technical Diversity:** Standardises protocols and documentation to reduce complexity and support platform governance.
- **Design for Interoperability:** Requires open standards and secure, modular integration.
- **Tier 1 Cloud SaaS First:** Prefers APIs from major vendors for scalable, secure, and sustainable service delivery.

### From AI Architecture Principles

- **Modular and Composable Design:** APIs must support modular integration and composability.
- **Lifecycle Traceability:** Governance and audit requirements ensure traceability across API lifecycle.
- **Secure-by-Design:** Security requirements enforce robust controls for data and operations.
- **Interoperability and Standards Alignment:** APIs must use open standards and support integration with enterprise platforms.
- **Scalable Infrastructure:** SLAs and performance requirements ensure APIs can scale with demand.
- **Model Portability and Reusability:** APIs should support portability and reuse, especially for AI and data-driven services.
- **Observability and Monitoring:** APIs must provide health checks and support monitoring for operational health.
- **Service Landing and Operational Readiness:** APIs must pass architecture and operational readiness checks before production use.
- **Governance Hooks:** APIs must expose metadata and interfaces for compliance and policy enforcement.
- **Strategic Alignment:** API selection and integration must align with organisational architecture and digital strategy.

## Principle Coverage Check

All requirements from both sets of principles are reflected in this standard. If a principle is not explicitly covered, it is addressed through the standard’s requirements for governance, compliance, resilience, interoperability, and strategic alignment. Any future updates to principles should be reviewed for impact on this standard.
