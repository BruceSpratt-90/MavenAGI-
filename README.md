# MavenAGI

Repository for Maven customer-support instructions, routing references, and application code.

## Purpose

This repository contains the Markdown control and knowledge references used to improve Maven’s customer answers, product routing, and support actions.

## Document architecture

| Layer | Canonical file | Responsibility | Load mode |
|---|---|---|---|
| Runtime control | `Core agent additional persona instructions.md` | Decision order, authentication enablement, evidence calibration, and action truthfulness | Always on |
| Workflow policy | `Escalation Protocol.md` | Escalation, intake, approval, submission, and post-case topic switching | Conditional |
| Product routing | `onetrust-product-taxonomy-revised.md` | Product names, aliases, packages, and product-specific evidence boundaries | Retrieval when relevant |
| Intent classification | `onetrust-capability-intent-disambiguation.md` | OneTrust capability versus Maven action | Retrieval when ambiguous |
| Case values | `OneTrust Support Case Taxonomy.md` | Valid Solution, Product, and Capability values | Case creation only |
| Response style | `OneTrust Agent Persona Instructions.md` | Response structure and troubleshooting presentation | Always on, concise |
| Brand voice | `OneTrust Brand Voice & Guardrails.md` | Tone, language, and high-level customer-facing boundaries | Always on, concise |

## Authority order

When guidance overlaps, apply this order:

1. Platform and connector capabilities, including action results.
2. Safety, security, authentication, and approval controls.
3. Runtime control in the Core document.
4. Escalation workflow.
5. Product, intent, and case-value references.
6. Persona and Brand style.

A lower layer must not override a higher layer.

## Maintenance rules

* Add a rule to the narrowest document that owns the concern.
* Do not duplicate runtime, escalation, product, or case rules in persona or brand files.
* When a product name, alias, capability, or case value changes, update the relevant reference and its tests.
* When escalation or action behaviour changes, update `Escalation Protocol.md` first.
* Every external knowledge or action dependency must have an owner, source location, and availability test.
* Remove references to documents that do not exist or are not deployed.

## Retrieval guidance

Do not load the full case taxonomy or escalation protocol for every message. Retrieve them when a case or escalation is relevant. Retrieve product and intent references based on the customer’s request. Keep always-on instructions short and behavioural.

## Testing expectations

Maintain regression tests for:

* product-boundary errors;
* OneTrust capability versus Maven action ambiguity;
* authentication unlock and authentication failure;
* incomplete evidence and qualified answers;
* case taxonomy clarification;
* approval and failed submission; and
* post-case topic switching.

## Change review checklist

Before merging a Markdown change, confirm:

* Does it have one clear owner and authority?
* Does it duplicate a rule elsewhere?
* Does it change the runtime decision order or an action contract?
* Does it require a new regression test?
* Is the source or dependency available in the deployed Maven context?
