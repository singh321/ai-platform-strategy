# Build vs Buy in AI Platforms

A product strategy framework for deciding when to build platform capabilities internally vs buy external tools.

---

## Why this matters

AI teams make build-vs-buy decisions constantly:
- model providers
- eval tooling
- vector databases
- orchestration layers
- observability tools
- safety layers

There is no universal right answer.
The right answer depends on leverage, differentiation, speed, and cost.

---

## My decision framework

I evaluate build vs buy using 5 lenses:

### 1. Strategic differentiation
If the capability is core to product differentiation, internal build becomes more attractive.

Examples:
- domain-specific ranking logic
- proprietary orchestration
- custom workflow intelligence

---

### 2. Speed to value
If buying helps launch faster without weakening the core product, it often makes sense.

Examples:
- managed vector DB
- third-party observability
- off-the-shelf moderation

---

### 3. Long-term cost and flexibility
Buying can be fast initially but costly later.
Building can be slow initially but create strategic control.

Questions:
- Will usage scale make vendor cost expensive?
- Will lock-in hurt future flexibility?
- How much customization will we need?

---

### 4. Internal capability
Do we have the team and focus to build this well?
A weak internal build is often worse than a strong bought solution.

---

### 5. Integration complexity
Sometimes buying multiple tools creates hidden integration overhead.

Questions:
- Will the tool fit our architecture?
- Will it increase fragmentation?
- Does it create operational complexity?

---

## What often makes sense to buy early

- foundation models
- basic eval tooling
- managed retrieval infrastructure
- moderation and safety tooling
- observability tools

---

## What often becomes build-worthy later

- workflow-specific orchestration
- business-specific ranking
- proprietary memory systems
- custom policy logic
- product-differentiating copilots and workflows

---

## Final principle

Buy where speed and standardization matter.
Build where differentiation, control, and long-term leverage matter.
