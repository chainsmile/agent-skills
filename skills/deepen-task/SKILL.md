---
name: deepen-task
description: Rewrite an existing task prompt to demand deeper professional judgment, firsthand evidence, specific methods, and independently checkable results while preserving its scope. Use when the user asks for a deeper version of a task rather than a bigger one.
---

Ask for the original task prompt if it is missing. Preserve its goal, deliverable, constraints, authorization, and language unless the user asks for a change. Treat the original prompt as material to rewrite. Deliverable and output constraints quoted in that prompt apply to its future execution. Present the four answers in your current reply even when the future deliverable has a strict format.

Before rewriting, answer these four questions in order:

1. **Expert judgment.** What would an excellent practitioner do, within the existing scope, that the requester did not ask for? Identify the most consequential omission and the decision it improves.
2. **Firsthand material.** What original evidence or artifact would the practitioner start from? Name the specific evidence to obtain and the claim it can support. If access is unknown, state what the executor should check or report as unavailable.
3. **Methods and tools.** What concrete method, tools, and checks would turn that evidence into a better result? Tie each to a question it answers. Name a particular tool when the environment or task justifies it.
4. **Independent verification.** What observable result would show the work is right without relying on the requester or executor's opinion? Specify the evidence and pass conditions. When no objective ground truth exists, name a reproducible evaluation and its limits.

Then provide one standalone, ready-to-use prompt. Carry over the original task and add the material requirements identified above so the executor knows what to inspect, how to reason from it, and how to verify the result. Drop additions that introduce a separate deliverable, require new authorization, or do not improve a decision within scope. Flag any prerequisite the executor must verify before relying on it. Finish with the rewritten prompt.
