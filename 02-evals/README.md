# Evaluation

Evaluation is the control system for production AI. Without a repeatable eval loop, prompt changes, retrieval changes, model upgrades, and agent modifications become guesswork.

## Evaluation layers

### Retrieval

Measure whether the right evidence was found.

Common metrics:

- Recall@K
- Precision@K
- Hit Rate
- MRR
- nDCG

### Generation

Measure whether the final answer is useful and grounded.

Typical dimensions:

- Correctness
- Faithfulness
- Relevance
- Completeness
- Citation correctness
- Abstention quality

### Agents

Evaluate more than the final answer:

- Tool selection
- Tool arguments
- Number of steps
- Recovery behavior
- Policy compliance
- Task completion
- Cost and latency

## Production loop

```text
Production failure
      ↓
Capture example
      ↓
Label / define expected behavior
      ↓
Add to eval dataset
      ↓
Reproduce
      ↓
Fix
      ↓
Regression test
      ↓
Deploy
```

## Principles

- Keep retrieval and generation evals separate.
- Prefer task-specific evals over generic scores.
- Validate LLM judges against human labels.
- Version datasets together with prompts and models.
- Run offline evals before deployment and online monitoring after deployment.
- Record failures, not just aggregate scores.
