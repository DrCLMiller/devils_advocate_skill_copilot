# devils_advocate_skill_copilot
MS Copilot agent skill that examines an idea, strategy, framework, etc. to help identify gaps and failure point.

-------
# 🔧 Installing the Devil's Advocate Agent in Copilot Studio

1. Download the `copilot-agent.json` file from this repository.
2. Open your Copilot Studio: https://copilot.microsoft.com/studio
3. Create a NEW Copilot.
4. In the left sidebar, open **Plugins / Skills**.
5. Click **Import Skill** or **Add Custom Skill**.
6. Upload the `copilot-agent.json` file.
7. Enable the skill once it appears in your Copilot.
8. Use it by prompting your Copilot with:
   - "Play devil's advocate on this plan..."
   - "Stress-test this idea..."
   - "Red-team this strategy..."
   - "What could go wrong?"

-------

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
