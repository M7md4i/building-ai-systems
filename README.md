# Building AI Systems

A practical, production-focused knowledge base for designing, building, evaluating, securing, and operating modern AI systems.

This repository is not a single application and it is not a framework tutorial. It is a growing collection of engineering notes, patterns, checklists, code snippets, experiments, incident write-ups, and reference architectures for real-world AI systems.

## Areas

| Area | Focus |
|---|---|
| [RAG](./01-rag/) | Retrieval, chunking, hybrid search, reranking, citations, indexing, ACLs |
| [Evaluation](./02-evals/) | Retrieval metrics, generation evals, LLM-as-a-judge, regression suites |
| [Agents](./03-agents/) | Tool design, workflows, memory, MCP, human-in-the-loop |
| [Context Engineering](./04-context-engineering/) | Context assembly, compression, memory, retrieval context, token budgets |
| [Security](./05-security/) | Prompt injection, RAG poisoning, tenant isolation, PII, sandboxing |
| [Observability](./06-observability/) | Tracing, metrics, logs, cost and quality monitoring |
| [Performance](./07-performance/) | Latency, TTFT, caching, batching, streaming, token optimization |
| [Data Pipelines](./08-data-pipelines/) | Ingestion, parsing, deduplication, queues, retries, idempotency |
| [Inference](./09-inference/) | Serving, vLLM, quantization, throughput, GPU utilization |
| [LLMOps](./10-llmops/) | Prompt/model versioning, routing, fallbacks, deployment lifecycle |
| [System Design](./11-system-design/) | Production architectures, multi-tenant AI, event-driven AI systems |
| [Production Incidents](./12-production-incidents/) | Failure modes, root causes, fixes, prevention |
| [Resources](./resources/) | Papers, blogs, books, tools, courses, case studies |

## Content types

Each topic should use the smallest format that adds value:

- **Article** — explain a production concept or decision.
- **Pattern** — reusable engineering approach with trade-offs.
- **Snippet** — focused implementation example.
- **Experiment** — measured comparison with dataset, metrics, and results.
- **Checklist** — pre-production or review criteria.
- **Incident** — symptom → root cause → fix → prevention.
- **Reference architecture** — system-level design and decision notes.

## Production-first principles

1. Measure quality before optimizing complexity.
2. Separate retrieval quality from generation quality.
3. Treat prompts, indexes, datasets, and models as versioned artifacts.
4. Build authorization into retrieval, not after retrieval.
5. Treat retrieved and tool-provided content as untrusted input.
6. Trace the full request path so failures are diagnosable.
7. Track latency, reliability, quality, and cost together.
8. Prefer simple workflows before autonomous agents.
9. Turn production failures into regression tests.
10. Document trade-offs and decisions, not only implementations.

## What a useful note should answer

- What problem does this solve?
- When should I use it?
- When should I avoid it?
- How do I measure whether it works?
- What does it cost in latency, complexity, or money?
- How can it fail in production?
- How do I operate and debug it?

## Roadmap

See [ROADMAP.md](./ROADMAP.md).

## Related repository

This repository focuses on AI-specific system concerns. General software architecture and production engineering belong in `building-software-systems`.

---

> The goal is not to collect AI buzzwords. The goal is to understand how to build AI systems that remain useful, measurable, secure, and operable after the demo.