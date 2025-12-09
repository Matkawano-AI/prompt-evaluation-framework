# Prompt Evaluation Framework

This repository outlines a **practical, lightweight approach** to evaluating
large language model (LLM) outputs when used in real workflows.

The focus is on **judgment and validation**, not model training or benchmarking.

## Why Output Evaluation Matters

LLMs can produce fluent responses that appear correct
but contain subtle errors, omissions, or violations of constraints.

In real workflows, unvalidated AI output can lead to:
- Silent logic errors
- Misleading recommendations
- Broken downstream processes

For this reason, prompt engineering must include
**explicit evaluation and validation steps**, not just generation.

## Practical Evaluation Checklist

Before using an AI-generated output in a real workflow, I evaluate it against
the following criteria:

1. **Goal Alignment**
   - Does the output actually address the stated objective?
   - Is it solving the right problem?

2. **Constraint Compliance**
   - Are all explicit constraints respected?
   - Is anything added that was explicitly excluded?

3. **Clarity & Specificity**
   - Are instructions or recommendations actionable?
   - Is vague language avoided?

4. **Logical Consistency**
   - Do the steps or arguments follow a clear, reasonable order?
   - Are there contradictions or gaps?

5. **Risk & Assumption Awareness**
   - Are assumptions made explicit (or at least reasonable)?
   - Would a wrong assumption cause downstream issues?

If any of these checks fail, the output is revised or discarded.
