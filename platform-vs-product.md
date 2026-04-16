# Platform vs Product

A practical framework for deciding what should be built as a shared platform capability vs a product-specific feature.

---

## Why this decision matters

As AI products grow, teams often see repeated needs across workflows:
- retrieval
- memory
- prompting
- evaluation
- logging
- feedback capture
- workflow orchestration
- access control

At some point, these repeated needs can become platform capabilities.

But platform thinking too early can slow teams down.
Platform thinking too late can create duplication and inconsistency.

The goal is to platformize at the right time.

---

## Product vs Platform

### Product layer
The product layer is where user-facing workflows live.

Examples:
- meeting prep
- email drafting
- support response generation
- lead enrichment
- AI copilots

The product layer is optimized for:
- user value
- workflow fit
- adoption
- differentiation

---

### Platform layer
The platform layer provides reusable capabilities used by multiple products or workflows.

Examples:
- prompt orchestration
- model routing
- eval framework
- retrieval layer
- memory system
- feedback pipeline
- policy / guardrail layer

The platform layer is optimized for:
- reuse
- consistency
- speed across teams
- governance
- scalability

---

## My decision framework

I use 5 questions:

### 1. Is this needed across multiple workflows?
If yes, platform potential increases.

### 2. Is there repeated implementation cost?
If teams keep rebuilding the same thing, that is a strong platform signal.

### 3. Does consistency matter?
Capabilities like guardrails, evals, permissions, or logging often benefit from consistency.

### 4. Will platformization increase future velocity?
Platform work should unlock multiple products, not only one team’s roadmap.

### 5. Is the pattern mature enough?
Do not platformize unstable patterns too early.

---

## What should usually remain product-specific

- UX details
- workflow-specific prompting
- user-facing interaction design
- context packaging for specific use cases
- vertical-specific business logic

These often need local optimization and fast iteration.

---

## What often belongs in platform

- model routing
- eval tooling
- retrieval infrastructure
- logging and observability
- feedback capture
- cost controls
- policy / guardrail frameworks
- identity and permissions foundations

---

## Common mistakes

### Mistake 1: Platformizing too early
Teams create abstraction before understanding real usage patterns.

### Mistake 2: Keeping everything in products
This creates duplication, cost, and inconsistent quality.

### Mistake 3: Platformizing UX
Shared back-end capabilities are often reusable. User experience usually is not.

---

## Final principle

Build platform where reuse, consistency, and leverage are real.

Keep product-specific where workflow differentiation and speed matter most.
