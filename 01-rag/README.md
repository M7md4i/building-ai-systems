# RAG

Retrieval-Augmented Generation is not just `embed → retrieve → prompt`. In production it is a search system, data pipeline, authorization boundary, evaluation problem, and operational workload.

## Topics

- Retrieval fundamentals
- Chunking strategies
- Embeddings
- Metadata design
- Hybrid search
- Reranking
- Query rewriting
- Citations and grounding
- Multi-tenant access control
- Index versioning and migration
- Retrieval evaluation
- Failure analysis

## Production baseline

A production RAG path should usually make these stages observable:

```text
Source
  ↓
Ingestion
  ↓
Parsing / normalization
  ↓
Chunking + metadata
  ↓
Embedding / indexing
  ↓
Query processing
  ↓
Authorization filters
  ↓
Retrieval
  ↓
Reranking
  ↓
Context construction
  ↓
Generation
  ↓
Citations / abstention
```

## Questions to answer before shipping

- What retrieval metric defines success?
- What is the evaluation dataset?
- How are document permissions enforced?
- How are deleted or updated documents propagated?
- How is an embedding model migration handled?
- Can the system abstain when evidence is weak?
- Are citations mapped to stable source identifiers?
- Can a trace explain why a particular chunk was selected?
- What is the P95 latency budget for retrieval and generation separately?
- What happens if the vector store or model provider fails?

## Planned notes

- `chunking-strategies.md`
- `hybrid-search.md`
- `reranking.md`
- `metadata-and-acl.md`
- `index-lifecycle.md`
- `retrieval-evaluation.md`
- `citations-and-grounding.md`

## Planned experiments

- Vector-only vs hybrid retrieval
- Chunk-size benchmark
- Reranker quality vs latency
- Metadata filtering impact
- Embedding model migration
