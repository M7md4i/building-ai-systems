# Roadmap

This roadmap is organized around production capability, not framework adoption.

## 01 — RAG

- Retrieval fundamentals
- Chunking strategies
- Embedding selection
- Metadata design
- Hybrid retrieval
- Reranking
- Query rewriting
- Citations and grounding
- Multi-tenant retrieval
- Index lifecycle and migrations

## 02 — Evaluation

- Golden datasets
- Retrieval metrics: Recall@K, Precision@K, MRR, nDCG
- Answer correctness and faithfulness
- Citation evaluation
- LLM-as-a-judge
- Human evaluation
- Regression suites
- Online evaluation

## 03 — Agents

- Workflow vs agent
- Tool contracts
- Tool calling
- Memory
- Human-in-the-loop
- MCP
- Multi-agent systems
- Long-running agents
- Failure recovery

## 04 — Context Engineering

- Context assembly
- Context budgets
- Compression
- Conversation history
- Retrieval context
- Tool result context
- Context prioritization

## 05 — Security

- Direct prompt injection
- Indirect prompt injection
- RAG poisoning
- Tenant isolation
- PII handling
- Tool authorization
- Secret handling
- Agent sandboxing

## 06 — Observability

- Request tracing
- Retrieval traces
- Model traces
- Token usage
- Cost attribution
- Latency breakdowns
- Quality monitoring
- Production feedback loops

## 07 — Performance

- TTFT
- End-to-end latency
- Streaming
- Caching
- Batching
- Model routing
- Context reduction
- Load testing

## 08 — Data Pipelines

- File ingestion
- Parsing
- Normalization
- Deduplication
- Idempotency
- Queue-based workers
- Retry policy
- Dead-letter queues
- Backfills

## 09 — Inference

- Hosted vs self-hosted models
- Serving architecture
- vLLM
- Quantization
- Batching
- GPU memory
- Throughput vs latency

## 10 — LLMOps

- Prompt versioning
- Model versioning
- Evaluation gates
- Model routing
- Fallbacks
- Canary releases
- Rollbacks
- Cost controls

## 11 — System Design

- Simple RAG service
- Enterprise RAG
- Multi-tenant AI systems
- Agent platform
- Event-driven AI
- AI gateway

## 12 — Production Incidents

Every incident note should capture:

1. Symptoms
2. Impact
3. Detection
4. Root cause
5. Fix
6. Prevention
7. Regression test added
