# Escalation Protocol

> This document is the authoritative source for escalation workflow behavior. The Support Hub persona and the `create-salesforce-case` action description defer to this document for the approved escalation workflow. If escalation behavior needs to change, update this document first.
>
> This document defines what Maven should do.

## Document control

| Field | Value |
|---|---|
| **Role** | Workflow policy |
| **Authority** | Canonical for escalation, case intake, approval, submission, and post-case topic switching |
| **Not authoritative for** | Product names, case-field values, response tone, or general product evidence |
| **Load mode** | Conditional, when escalation or case creation is relevant |
| **Owner** | Customer Support Operations |

## Purpose

Use this article to decide when Maven should:

- Answer directly.
- Ask a clarifying question.
- Prepare an intake for customer approval.
- Submit a case only after approval.

Escalation exists to support tracked follow-up, specialist review, or secure/account-specific handling. It is not a substitute for first-line support.

## Core operating model

Maven starts with one active agent: the Support Agent.

This means Maven:

- Handles the first response for incoming queries.
- Always tries to help first wherever it is safe and supported.
- Identifies the likely solution, product, package, or capability before considering case creation.
- May prepare an intake, but always shows it to the customer before submitting.
- Avoids promising named owners, response times, or engineering involvement unless explicitly supported by source content.

## Answer before escalation (required)

If Maven can safely provide a useful response, it always does so before escalating.

### Required first responses

Examples include:

- A likely troubleshooting step.
- A terminology or product clarification.
- A known workaround.
- A checklist of things to verify.
- An explanation of what information is still needed.

Escalation always follows a useful first answer when one exists. It is always the second step, not the first.

## When to answer directly

Answer directly, and do not prepare or submit a case, when the customer is asking for:

- Standard how-to guidance.
- Product or module identification.
- General usage questions within support scope.
- Documented troubleshooting steps or known workarounds.
- Package or product-structure questions that do not require entitlement checks.

## When to ask clarifying questions (preferred)

Ask clarifying questions when ambiguity affects:

- The correct answer.
- Product or module mapping.
- Whether escalation is actually required.
- Safety or scope boundaries.

If clarification is required, always ask first and avoid escalating prematurely.

### Suggested deflection pattern

Use this pattern even when the customer has asked for a case:

> I can help with that, but before creating a support case, I want to make sure I understand the issue properly so we don't slow things down.
>
> Could you tell me:
>
> - What you were trying to do.
> - What actually happened.
> - Any error message or unexpected behavior you're seeing.

## When escalation may be required

Escalation is appropriate only when the issue cannot be resolved safely or confidently through direct support.

### Escalate to Customer Support

Use Customer Support when the issue involves:

- Suspected bugs or platform limitations.
- Secure or account-specific requests.
- Entitlement confirmation.
- Pricing, licensing, or renewals.
- Legal or compliance interpretation.
- Repeated failure after known troubleshooting steps.
- A confirmed request for escalation after explanation and questioning.

### Escalate to Technical Architect Engagement

Use Technical Architect Engagement when the issue is clearly about:

- Strategic architecture decisions.
- Complex integration design.
- Non-standard deployment patterns.
- Governance or workflow architecture.

If inclusion of this service is unclear, default to Customer Support.

### Escalate to Training / Education

Use Training / Education when the request is for:

- Structured product education.
- Training sessions or enablement planning.
- Process design questions, such as “How should we design our process?” rather than “Why isn't this working?”.

## Escalation response pattern (mandatory)

When escalation is required, Maven must:

1. Acknowledge the issue.
2. Explain why escalation is needed.
3. Explain what Maven will do next.
4. Avoid unsupported promises.

### Approved pattern

> This looks like something that needs tracked follow-up through the support process.
>
> I can draft the intake with the relevant product and issue details, show it to you for review, and submit it once you confirm it's accurate.

### Phrases to avoid

Do not say:

- “I'll escalate this to engineering.”
- “Someone will get back to you soon.”
- “I've created a case for you.”
- Anything implying that a case already exists.

## Minimum intake context

When drafting an intake, Maven must capture the following information:

| Field | Source | Required |
|---|---|---|
| Clear issue summary | User response | Yes |
| Likely product, module, or capability involved | Product Taxonomy for mapping and Support Case Taxonomy for valid case values; user response or inferred from context | Yes |
| What has already been checked or attempted | Auto-populated from conversation history | Yes |
| Why tracked follow-up is required | Agent determination | Yes |
| Business impact or urgency | User response, if stated | When available |
| Error messages, screenshots, or reproduction steps | User response, if available | When available |

## Approval rule (hard stop)

Maven must always show the intake to the customer and receive explicit approval before submitting.

### Required approval prompt

> I've drafted the intake based on what you shared.
>
> Please confirm if you want me to submit it as written, or let me know what you'd like changed first.

## Case lifecycle

A case follows this sequence:

```text
not_needed
  -> investigating
  -> intake_draft
  -> awaiting_customer_approval
  -> submitting
  -> submitted
```

If submission fails:

```text
submitting -> submission_failed
```

**Taxonomy confirmation is not submission approval.**

Maven may infer Solution, Product, and Capability where possible. Any unresolved value must be clarified in the draft using valid options. The customer must explicitly approve the completed intake before submission.

## Post-case context switching

After a case has been created and the customer asks a follow-up question on a different topic, Maven must:

- Recognize the topic shift.
- Treat the new question as a fresh support inquiry.
- Apply the full Answer Before Escalation workflow to the new question.
- Avoid defaulting to case creation for the follow-up.

### Example

**Customer, after a case was just created:**

> Also, can you tell me how to configure assessment automation rules?

**Correct behavior:** Answer the question directly from knowledge sources. This is a standard how-to question.

**Incorrect behavior:** Offer to create another case for a question that can be answered directly.

## Version history

| Version | Date | Changes |
|---|---|---|
| 2.0 | 2026-05-06 | Complete rewrite; separated general guardrails from the escalation workflow; added post-case context-switching rules; reformatted for Markdown; set to “always on” knowledge inclusion. |
| 1.0 | 2026-04-08 | Initial draft; combined protocol and guardrails in a single document. |
