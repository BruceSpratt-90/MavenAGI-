# OneTrust Product Taxonomy

## Document control

| Field | Value |
|---|---|
| Audience | Maven Support Agent |
| Scope | Product identification, routing, knowledge retrieval, and customer guidance |
| Status | Active guidance |
| Version | 3.0 |
| Last reviewed | 15 September 2026 |
| Owner | Customer Support Operations / Product Knowledge Management |
| Authority | Product, solution, capability, alias, package, and product-specific evidence boundaries |
| Not authoritative for | Case submission workflow, response tone, or Maven action execution |
| Load mode | Retrieve when product identification or product capability evidence is relevant |

## Handoffs

* Use [Capability-Question Disambiguation](onetrust-capability-intent-disambiguation.md) to determine whether the customer is asking about OneTrust functionality or a Maven action.
* Use this document to map OneTrust product language and establish the product-specific evidence boundary.
* Use [Support Case Taxonomy](OneTrust%20Support%20Case%20Taxonomy.md) for valid case-field values.
* Use [Escalation Protocol](Escalation%20Protocol.md) for case drafting, approval, and submission.

## Purpose

Use this article to:

* identify the relevant OneTrust solution, product, capability, or package;
* map customer language to approved terminology;
* support product-level routing and knowledge retrieval;
* use consistent product names in customer responses; and
* prevent unsupported capability assumptions between products.

This is a product and routing reference. It is not a licence, entitlement, contract, or feature-availability source.

## Taxonomy model

The operational taxonomy is:

```text
Platform
└── Solution
    └── Product
        └── Capability
```

Packages are a separate commercial overlay:

```text
Package
└── Included products and capabilities
```

Packages are not a strict child level beneath capabilities.

## Operating principles

* Identify the likely solution when it helps orient the request.
* Identify the most specific product supported by the customer’s language.
* Identify the capability when it improves retrieval, troubleshooting, or routing.
* Treat package names as commercial signals, not proof of entitlement or feature availability.
* Use approved current routing values for case categorisation.
* Use approved customer-facing terminology where it differs from an internal routing value.
* Preserve recognised aliases and legacy names so Maven can understand customer language.
* Ask a clarifying question when ambiguity would materially change the answer or routing.
* Do not expose taxonomy detail unless it helps answer the customer’s question.

## Product anchoring and evidence boundary

The product explicitly named or clearly identified in the customer prompt is the response anchor. Product-specific documentation is required to support claims about that product’s capabilities or behaviour.

This is an evidence boundary, not a rigid response workflow.

* Do not infer that a capability in one product exists in another product.
* Do not transfer functionality, behaviour, configuration steps, limitations, integrations, or entitlement between products.
* A shared solution, package, platform, use case, technology, or capability name is not evidence that products work the same way.
* Documentation for an adjacent product may provide context, but it is not sufficient proof for the named product.
* Use aliases and legacy names to find relevant content, but confirm that the source clearly applies to the named product before using it as evidence.
* If documentation directly confirms the capability, answer clearly.
* If evidence is partial or ambiguous, distinguish confirmed information from uncertainty.
* If direct evidence is unavailable, qualify the limitation, ask a focused question, or route to support.
* Do not present an inference as confirmed functionality for the named product.
* For comparisons, use product-specific evidence for each product.

Before making a product capability claim, Maven should be able to identify:

1. The product named or resolved from the customer’s language.
2. The product-specific source used as evidence.
3. The capability or function that source confirms.

This is a quality check, not a requirement to expose the process to the customer.

## Solutions

| Solution | Customer-facing purpose | Key aliases or notes |
|---|---|---|
| Consent & Preferences | Consent capture, preference management, and consent experiences | Consent, CMP, UCPM, preference centre |
| Privacy Automation | Privacy operations, data mapping, assessments, incidents, notices, and data subject requests | Privacy Ops, privacy automation |
| Data & AI Governance | Data discovery, classification, data governance, and AI governance | Data Use Governance is a recognised customer-facing alias pending final naming governance |
| Tech Risk & Compliance | Compliance, policy, audit, IT risk, and control management | GRC, tech risk, compliance automation |
| Third-Party Management | Vendor lifecycle, third-party risk, screening, due diligence, and monitoring | TPRM, third-party risk, vendor risk |
| Platform | Shared platform capabilities, access, integrations, email, and AI services | Platform support |
| Account Management | Account, subscription, user, performance, and general account administration | Account query, admin, billing |

### Data & AI Governance naming note

Current sources use both **Data & AI Governance** and **Data Use Governance**.

Until a single canonical customer-facing name is confirmed:

* use **Data & AI Governance** for operational routing;
* recognise **Data Use Governance** as an alias;
* do not describe either term as definitively legacy; and
* use the terminology present in the relevant approved customer-facing source when responding.

## Products and capabilities

This product map supports routing and retrieval. It is not a complete feature catalogue.

### Consent & Preferences

| Product | Representative capabilities and terms |
|---|---|
| Universal Consent & Preference Management | Preference management, consent experiences, public APIs, integrations, dashboards, and bulk actions |
| Consent Management (CMP) | Consent services, consent SDK, scanning and detection, consent experience, third-party integrations, and dashboards |

Use **CMP** for cookie-banner and consent-management questions. Use **UCPM** for preference-centre and preference-management questions. Clarify when “consent” is used broadly.

### Privacy Automation

| Product | Representative capabilities and terms |
|---|---|
| Data Mapping Automation | Inventory, personal data, data lineage, cross-border mapping, assessments, automation rules, and dashboards |
| Assessment Automation | Assessments, templates, logic, workflows, routing rules, projects, automation rules, and dashboards |
| Privacy Incident Management | Incident register, assessments, workflows, routing rules, web forms, automation rules, and dashboards |
| Privacy Notice Management | Privacy notices, templates, workflows, SDK integration, share links, change tracking, consent integration, and dashboards |
| DataGuidance | Regulatory content and intelligence |
| Data Subject Request (DSR) Automation | Data subject and trust portal, web forms, workflows, requests, subtasks, response templates, translations, identity verification, and dashboards |
| Data Redaction | Redaction preferences, redaction workspace, file upload, discovery, and classification |
| Privacy Operations | Customer-facing umbrella term; narrow to the specific product when the customer’s intent supports it |

“Privacy Operations” should not automatically be used as the final product when the customer has identified a specific product area.

### Data & AI Governance

| Product | Representative capabilities and terms |
|---|---|
| Data Discovery & Classification | Control centre, gallery, worker node, scan management, data sources, scan profiles, classifiers, classification profiles, automation rules, terms, identity graph, and dashboards |
| AI Governance | AI inventory, assessments, workflows, transparency reporting, model gallery and model cards, AI integrations, automations, and dashboards |

### Tech Risk & Compliance

| Product | Representative capabilities and terms |
|---|---|
| Compliance Automation | Compliance initiatives, controls, evidence tasks, standards and frameworks, automated evidence collection, workflows, and dashboards |
| Audit Management | Audits, workpapers, findings, audit tasks, workflows, automation rules, and permissions |
| Enterprise Policy Management | Standards, policies, procedures, attestations, exceptions, templates, workflows, automation rules, and dashboards |
| IT Risk Management | Risk register, risk hierarchy, controls, evidence tasks, issues, assessments, inventories, libraries, workflows, automation rules, and dashboards |
| Certification Automation | Migration, readiness, audits, findings, risk, compliance portfolio, policies, procedures, controls, evidence, integrations, and assurance tools |

Treat Certification Automation as a migration or legacy product only when the customer’s context supports that interpretation.

### Third-Party Management

| Product | Representative capabilities and terms |
|---|---|
| Third-Party Risk Management | Inventories, vendors, engagements, contracts, issues, assessments, workflows, automation rules, and dashboards |
| Third-Party Risk Exchange | Exchange, breach and incident newsfeeds, and vendor scores |
| Third-Party Due Diligence | Screening and monitoring, usage tracking, assessments, enhanced due diligence services, integrations, workflows, and dashboards |

Use Third-Party Risk Management for the broader vendor lifecycle. Use Third-Party Due Diligence for screening and due diligence. Use Third-Party Risk Exchange for external risk intelligence and vendor scores.

### Platform and Account Management

| Area | Representative areas |
|---|---|
| Platform | Access management, email and branding, integrations and automation, and artificial intelligence |
| Account Management | Account query, performance, user management, data import, general settings, user preferences, language, support, hosting, and related account administration |

Include these areas in routing when they are within Maven’s support scope.

## Package guidance

Customers may refer to packages instead of products or capabilities. Treat package mentions as routing and retrieval signals only.

| Customer mention | Likely interpretation |
|---|---|
| UCPM | Universal Consent & Preference Management |
| CMP Base | Consent Management Platform base package |
| CMP Suite | Consent Management Platform suite |
| Privacy Automation | Privacy Automation package or solution-level reference |
| Privacy Automation Suite | Broader Privacy Automation package reference |
| Third-Party Risk Management | Third-party risk package or product reference |
| Third-Party Management | Broader third-party management package or solution reference |

### Package rules

* Do not treat a package mention as proof of entitlement.
* Do not infer exact included features from a package name alone.
* Narrow to the product and capability when the answer depends on it.
* Use approved pricing, contract, or account sources for entitlement questions.
* If the customer asks what is included, explain the likely package context but state that account-specific confirmation is required.

## Customer language mapping

| Customer says | Map to | Guidance |
|---|---|---|
| Cookie banner | Consent Management (CMP) | Use CMP unless the customer means preference management. |
| CMP | Consent Management (CMP) | Product acronym. |
| Preference centre / preference center | Universal Consent & Preference Management | Usually preference management. |
| UCPM | Universal Consent & Preference Management | Product or package shorthand. |
| Privacy Ops | Privacy Operations | Umbrella term; narrow to the specific product when possible. |
| Privacy Automation | Privacy Automation | Solution or package-level reference, not automatically one product. |
| DSR / DSAR automation | Data Subject Request (DSR) Automation | Route within Privacy Automation. |
| Data mapping | Data Mapping Automation | Use when the customer means mapping, inventory, lineage, or cross-border mapping. |
| Assessment automation | Assessment Automation | Route to the assessment product. |
| Privacy incident | Privacy Incident Management | Route to the incident product. |
| Privacy notice | Privacy Notice Management | Route to the notice product. |
| DataGuidance | DataGuidance | Product name. |
| AI inventory | AI Governance | Capability-level intent. |
| Model cards | AI Governance | Capability-level intent; use product-specific evidence. |
| IT risk | IT Risk Management | Product shorthand. |
| Compliance automation | Compliance Automation | Clarify if the customer means policy, audit, evidence, or controls. |
| Vendor risk / TPRM | Third-Party Risk Management | Use for the broader vendor lifecycle. |
| Risk Exchange | Third-Party Risk Exchange | Product shorthand. |
| Due diligence | Third-Party Due Diligence | Clarify if the customer means the broader TPRM lifecycle. |
| Data Use Governance | Data & AI Governance | Recognised alias pending final naming governance. |
| Data & AI Governance | Data & AI Governance | Operational routing name. |
| Platform | Platform | Shared platform intent. |
| Account query / billing / subscription | Account Management | Account-level intent. |

## Routing guidance

1. Identify whether the customer has named a specific product.
2. If a product is named, use it as the response and retrieval anchor.
3. Identify the likely solution or shared platform area for context.
4. Identify the relevant capability within the anchored product when useful.
5. Identify a package only when the customer is speaking commercially or broadly.
6. Treat entitlement questions separately from product capability questions.
7. If the product is unclear and the distinction matters, ask one focused question.
8. If multiple products are named, keep their functionality and evidence separate.

## Retrieval and response guidance

For customer-facing product answers, prefer published customer-visible product documentation. Use broader solution or platform content for context, terminology, or navigation, but not as proof that a named product supports a capability.

When responding:

* use the approved current product name once the intent is clear;
* state the anchored product when useful;
* answer the customer’s practical question rather than explaining the taxonomy;
* distinguish confirmed information from uncertainty;
* avoid transferring functionality, limitations, workflows, or configuration steps between products;
* do not overstate feature availability or package inclusion; and
* provide a qualified answer, clarification, or support path according to what best serves the customer.

## Maintenance

Review this article when:

* product or capability names change;
* customer-facing product navigation changes;
* packages or pricing change;
* a new product, capability, or major alias is introduced; or
* Maven retrieval or routing shows repeated ambiguity.

## Public references

* [Products | OneTrust](https://www.onetrust.com/products/)
* [Pricing and Packaging | OneTrust](https://www.onetrust.com/pricing/)
