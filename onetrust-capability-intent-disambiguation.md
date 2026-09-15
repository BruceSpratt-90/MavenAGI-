# OneTrust Capability-Question Disambiguation

## Document control

* **Role:** Intent classification reference
* **Authority:** Canonical for distinguishing OneTrust capability questions from Maven action questions
* **Not authoritative for:** Product hierarchy, case values, escalation workflow, or response tone
* **Load mode:** Retrieval when request intent is ambiguous
* **Owner:** Customer Support Operations / Maven Implementation

## Purpose

Customers may use “can you” to ask either what OneTrust can do or what Maven can do. This document determines the subject of the question before product mapping and action selection.

## Core interpretation rule

* If the request concerns a OneTrust product capability, workflow, configuration, feature, integration, or business outcome, treat it as a OneTrust product question.
* If the request asks Maven to look up, create, update, attach, connect, submit, or explain its own behaviour, treat it as a Maven capability or action question.
* If the distinction matters and cannot be resolved from context, ask one focused question.

## OneTrust capability signals

Examples include:

* “Can OneTrust automate data subject requests?”
* “Can I configure risk scoring in IT Risk Management?”
* “Does Consent Management support mobile consent?”
* “Can we create a data map?”
* “Can we integrate this workflow?”

For these requests, hand off to [OneTrust Product Taxonomy](https://raw.githubusercontent.com/BruceSpratt-90/MavenAGI-/main/onetrust-product-taxonomy-revised.md) for product mapping and product-specific evidence.

## Maven action signals

Examples include:

* “Can you look up my open support case?”
* “Can you create a support case?”
* “Can you connect me to a person?”
* “Can you attach this file to my case?”
* “Can you check my account?”
* “What can you do?”

Maven must answer these questions honestly and must not imply that an action completed unless the approved workflow returned a successful result.

## Ambiguous requests

| Customer request | Handling |
|---|---|
| “Can you automate DSARs?” | Treat as a OneTrust capability question; map the product and use product-specific evidence. |
| “Can you create a case for me?” | Treat as a Maven action request; follow Escalation Protocol. |
| “Can you check whether I have access?” | Treat as an account or entitlement request; do not infer entitlement. |
| “Can you configure risk scoring?” | Clarify the product only if the answer differs by product. |
| “Can you search my knowledge base?” | Clarify whether the customer means Maven retrieval or a OneTrust product search function. |

## Guardrails

* Do not answer about Maven’s AI limitations when the customer is asking what OneTrust can do.
* Do not make a product capability claim without product-specific evidence.
* Do not transfer functionality, configuration, limitations, integrations, or entitlement between products.
* Do not use a package or solution name as proof of a product capability.
* Do not claim that an action completed when it did not.
* Use Escalation Protocol for support-case workflow and approval.
