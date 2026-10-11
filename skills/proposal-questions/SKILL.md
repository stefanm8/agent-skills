---
name: proposal-questions
description: >-
  Before asking the user a question, explain the semantics, components, and
  system the question refers to, then ask the question as a proposal with
  motivation and alternatives. Use whenever you are about to ask the user a
  question or request a decision, including when calling AskQuestion.
---

# Proposal Questions

Anytime you want to ask the user a question, explain what it refers to first, then ask the question as a proposal. Still ask with the normal question tool and follow that tool's instructions.

Do this for every question, including a question inside a larger task. If you can resolve the decision from the request, the code, or a sensible default, do not ask.

## Mental Model

Explain the thing the question is about through:

- **Semantics** — what the terms, states, and decisions mean here. Define any word that could be read more than one way.
- **Components** — the concrete pieces involved: modules, types, files, services, data, or interfaces. Name the real ones.
- **System** — how those pieces fit together, and what changes if the decision goes one way or another.

## The question is a proposal

Write the question as a proposal.

- **Motivation** — why this decision is being raised, what it unblocks, and what stays unresolved if it is not made.
- **Alternatives** — each real option, what it changes, and the tradeoff. Include the alternative you recommend.

Except, when there is an obvious true or false, such as requesting permissions

## Example

```markdown

## Motivation

## Alternatives

## Definitions

## Proposal
```

