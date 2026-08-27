# devils_advocate_skill_copilot
![CI](https://github.com/DrCLMiller/devils_advocate_skill_copilot/actions/workflows/CI.yml/badge.svg)
MS Copilot agent skill that examines an idea, strategy, framework, etc. to help identify gaps and failure point.

# Devil's Advocate Copilot Agent

**Name:** `devils-advocate`  
**Purpose:** A structured adversarial-analysis agent that stress-tests plans, strategies, and decisions by challenging assumptions and surfacing failure modes.

Use this agent whenever you want to:
- "play devil's advocate"
- "poke holes in" a plan
- "pressure-test" or "red-team" an idea
- ask "what could go wrong?" or "what am I missing?"
- get critical feedback before committing to a strategy

This agent does **not** provide encouragement or validation. Its sole purpose is adversarial critique.

---

## 🔧 Installation

1. Download or clone this repository.
2. Import `copilot-agent.json` into your Copilot environment.
3. Enable the agent in your Copilot settings.

---

## 🧠 What This Agent Does

This agent runs a **five-step adversarial workflow**:

### 1. Adversarial Analysis
Restates the plan, identifies stakes, and frames the environment.

### 2. Challenge Assumptions
Surfaces load-bearing assumptions and interrogates their validity.

### 3. Pre-Mortem
Assumes the plan failed and enumerates plausible causes.

### 4. Failure Tree Analysis
Breaks causes into structured failure paths (trigger → mechanism → consequence).

### 5. Synthesis: Top Objections
Ranks the strongest objections and highlights the biggest blind spot.

---

## 📝 Output Template

```markdown
## Adversarial Analysis
[plan restated, stakes, context]

## Challenge Assumptions
- [assumption] — [basis / risk if wrong]
...

## Pre-Mortem
- [cause]
...

## Failure Tree Analysis
Path 1: [trigger] → [mechanism] → [consequence]
Path 2: ...

## Synthesis: Top Objections
1. [objection] — mitigation: [...]
2. [objection] — mitigation: [...]
...

Biggest blind spot: [...]
