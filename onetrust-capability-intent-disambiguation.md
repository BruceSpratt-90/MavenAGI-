# OneTrust Capability-Question Disambiguation

Audience: Maven Support Agent  
Applies to: Intent interpretation before product identification and knowledge retrieval  
Status: Active guidance  
Version: 3.0  
Last reviewed: September 15, 2026  
Owner: Customer Support Operations / Maven Implementation

## Purpose

Customers often ask questions such as:

- “Can you do this?”
- “Do you support X?”
- “Is there a way to configure this?”
- “Does OneTrust have this capability?”

The phrase “can you” may refer either to:

- a capability of an identified OneTrust product, or
- an action Maven itself can perform.

This article determines the subject of the question. It does not determine the OneTrust product, capability, entitlement, or technical answer.

## Core interpretation rule

When “can you” refers to a OneTrust product capability, workflow, configuration, feature, or business outcome, interpret the question as a question about OneTrust.

When “can you” refers to an action Maven may perform in the conversation, interpret the question as a Maven capability or action question.

Do not answer about Maven’s own AI limitations when the customer is clearly asking what OneTrust can do.

## Likely OneTrust capability questions

Normally interpret the following as OneTrust product questions when the request concerns a product capability or business outcome:

- “Can you do [X]?”
- “Do you support [X]?”
- “Is it possible to [X]?”
- “Does OneTrust have [X]?”
- “Can I configure [X]?”
- “Can I manage [X] in OneTrust?”
- “Is there a way to [X]?”
- “Does this feature exist?”
- “Can we automate [X]?”
- “Can we integrate [X]?”

Examples:

- “Can OneTrust automate data subject requests?”
- “Can I configure risk scoring in IT Risk Management?”
- “Does Consent Management support mobile consent?”
- “Can we create a data map?”

For these questions, identify the likely product and use product-specific evidence before making a product capability claim.

## Maven capability or action questions

Interpret the request as being about Maven when the customer is asking Maven to perform an action or explain its own behaviour.

Examples include:

- “Can you look up my open support case?”
- “Can you create a support case?”
- “Can you connect me to a person?”
- “Can you attach this file to my case?”
- “Can you check my account?”
- “Can you change my tenant settings?”
- “What can you do?”
- “Are you the OneTrust chatbot?”
- “Can Maven search my cases?”

Maven must answer these questions honestly. It must not imply that an action was completed unless an approved workflow actually completed it.

## Ambiguous requests

Some requests can refer either to a OneTrust capability or a Maven action.


| Customer request                       | Likely interpretation                | Helpful handling                                                                          |
| -------------------------------------- | ------------------------------------ | ----------------------------------------------------------------------------------------- |
| “Can you automate DSARs?”              | OneTrust capability                  | Identify the likely product and answer from product-specific evidence.                    |
| “Can you create a case for me?”        | Maven action                         | Explain whether Maven can prepare or submit a case.                                       |
| “Can you check whether I have access?” | Account or entitlement question      | Do not infer entitlement. Use the approved account or support path.                       |
| “Can you configure risk scoring?”      | OneTrust capability, product unclear | Clarify the relevant product if the answer could differ by product.                       |
| “Can you search my knowledge base?”    | Maven or product action              | Clarify whether the customer means Maven retrieval or a OneTrust product search function. |
| “Can you delete this data?”            | Product workflow or Maven action     | Clarify the intended product, data, and requested action when necessary.                  |


When ambiguity matters, ask one focused question. Do not default to a generic Maven limitation when the customer is probably asking about OneTrust functionality.

## Handoff to the Product Taxonomy

Capability-question disambiguation and product taxonomy are separate controls:

1. Determine whether the customer is asking about OneTrust or Maven.
2. Use the Product Taxonomy to identify the relevant OneTrust solution, product, and capability.
3. Use product-specific knowledge to establish what the named product supports.
4. Respond in a way that is useful for the customer’s actual question.
5. Clarify or route when the evidence or scope is insufficient.

If the customer names a product, treat that product as the response anchor. Do not transfer functionality, behaviour, configuration steps, limitations, integrations, or entitlement from another product merely because the products share a solution, use case, platform, or similar capability name.

If the customer does not name a product and more than one product could support the request, clarify only when the distinction would change the answer. A safe, qualified answer is preferable to unnecessary questioning.

## Product-specific evidence and calibrated responses

Product-specific documentation is required to support claims about a named product’s capabilities or behaviour. This is an evidence boundary, not a rigid response script.

- Use documentation that clearly applies to the named product as the primary evidence for product-specific claims.
- General solution, platform, package, or adjacent-product content may help resolve terminology or provide context, but it must not be used to assert that the named product supports the same functionality.
- Do not transfer functionality, behaviour, configuration steps, limitations, integrations, or entitlement between products.
- If documentation directly confirms the capability, answer clearly and helpfully.
- If evidence is partial or ambiguous, distinguish what is confirmed from what is uncertain rather than forcing a yes/no answer.
- If direct product-specific evidence is unavailable, qualify the limitation, ask a focused question, or route to support, depending on what best serves the customer.
- Do not present an inference as confirmed product behaviour.
- Do not force clarification when the likely product mapping is clear and a safe, qualified answer is possible.
- For comparisons, use product-specific evidence for each product and keep the comparison explicit.

A useful response may contain context from broader sources, but any claim that a named product supports a capability must be grounded in documentation for that product.

## Response guidance

### OneTrust product capability question

A useful response will usually identify the likely product, use product-specific evidence, answer the customer’s practical question, and state relevant limitations or prerequisites. It does not need to expose the classification process.

Example:

> Customer: “Can OneTrust automate data subject requests?”
>
> Response approach: Identify the likely DSR product, retrieve product-specific evidence, and explain only the capabilities confirmed for that product. Do not substitute capabilities from another product or solution.

### Maven action question

A useful response will explain what Maven can or cannot do, avoid claiming an action was completed when it was not, and provide the next available path.

Example:

> Customer: “Can you look up my open support case?”
>
> Response approach: Answer about Maven’s case-lookup capability and provide the approved next step if lookup is unavailable.

### Product unclear

Use a focused clarification when needed:

> “Which OneTrust product are you referring to? The answer may differ by product.”

## Product-boundary examples

- If the customer asks about Consent Management, do not answer with Universal Consent & Preference Management behaviour unless the customer asks for a comparison or product-specific evidence confirms that the behaviour applies to Consent Management.
- If the customer asks about IT Risk Management, do not assume that behaviour from Compliance Automation or Enterprise Policy Management also applies to IT Risk Management.
- If the customer asks about Data Subject Request Automation, do not assume that a capability from Data Redaction or Data Mapping Automation is available or behaves the same way in Data Subject Request Automation.
- If the customer names a package rather than a product, identify the relevant product before making product-specific claims.

## Decision framework


| Customer intent signal                                                      | Interpretation                     | Helpful response approach                                           |
| --------------------------------------------------------------------------- | ---------------------------------- | ------------------------------------------------------------------- |
| Asks about a product feature, workflow, or configuration                    | OneTrust product question          | Identify the product and use product-specific knowledge.            |
| Asks whether OneTrust supports a business capability                        | OneTrust product question          | Map to the relevant product when needed, then answer from evidence. |
| Names a product explicitly                                                  | Product-anchored OneTrust question | Treat the named product as the response and retrieval boundary.     |
| Asks Maven to look up, create, update, attach, connect, or submit something | Maven action question              | Answer about Maven’s actual action capability.                      |
| Asks what Maven can do                                                      | Maven capability question          | Describe Maven’s approved scope honestly.                           |
| Asks about account access, entitlement, or subscription                     | Account or entitlement question    | Do not infer entitlement. Use the approved account or support path. |
| Ambiguous between OneTrust and Maven                                        | Unresolved intent                  | Ask one focused question if the distinction matters.                |
| Ambiguous between two or more OneTrust products                             | Unresolved product                 | Clarify if the distinction would change the answer.                 |


## Guardrails

Maven should not:

- answer about its own AI limitations when the customer is asking about OneTrust functionality
- assume that “can you” always means OneTrust or always means Maven
- make a product capability claim without product-specific evidence
- transfer functionality from one product to another
- use a package or solution name as proof of a product capability
- confirm entitlement from this article
- claim that an action was completed when it was not completed
- invent configuration paths, feature names, or product support
- turn an incomplete answer into a definitive “yes” or “no” when the evidence does not support it

## Maintenance

Review this article when customer phrasing, Maven actions, product names, retrieval behaviour, or support scope changes.