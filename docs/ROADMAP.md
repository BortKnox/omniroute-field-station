# ROADMAP

**From a mind map to a tool that streamlines the whole pipeline.**

```
STATUS   DRAFT — A DIRECTION, EDIT FREELY
```

The station is the thinking. A tool comes only after each stage of the pipeline is understood well enough to
automate without hiding what it does.

## PHASES

| Phase | Name | State | What it means |
|---|---|---|---|
| **01** | Field station | done | A playable map of the pipeline: harness, private link, gateway, providers, context filtering. |
| **02** | Pipeline spec | next | Write each stage down: inputs, outputs, how to check it works, how it fails. One page per stage. |
| **03** | Checklist, then script | planned | Turn the spec into a checklist a person can follow, then into a script that does the repeatable steps and verifies each hop. |
| **04** | One tool | idea | A single front end that provisions, wires, verifies and monitors the chain, and explains what it just did. |

## PRINCIPLES

- Explain before automating. A step that cannot be shown in the station is not ready to hide in a tool.
- Never ship credentials or default keys. Anything secret stays on the user's own machine or host.
- Keep the front door closed by default. The private link comes before any public exposure.
- Be honest about limits: free tiers, memory budgets and provider terms are part of the design.
- Verify each hop. Success means a request actually travelled the whole chain.

## OPEN QUESTIONS

- Which stages are worth automating first, and which should stay manual on purpose?
- What is the smallest host that runs the gateway reliably, measured and not assumed?
- How should the tool surface failures from third-party services it does not control?
