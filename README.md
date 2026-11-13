# HNSW vs IVF Index Benchmark for Semantic Product Search

## Project Information

- **Course:** Generative AI and AI Platform Engineering
- **Course code:** 25CS2207E
- **Section:** 8
- **Academic year:** 2026–2027
- **Institution:** Koneru Lakshmaiah Education Foundation
- **Supervisor:** Shaik Asif Sir

## Team

- **Simi Ayana** — 2520030254
- **Yuvan** — 2520030310

## Project Summary

This project will compare HNSW and IVF-Flat, two approximate nearest-neighbor indexing methods, for semantic product search. Product text and search queries will be converted into embeddings. Using the same data and hardware, we will compare retrieval quality, query speed, index build time, and memory use.

## Proposed Approach

We plan to use English query–product data from the Amazon Shopping Queries (ESCI) dataset, the `all-MiniLM-L6-v2` embedding model, and FAISS. Exact vector search will provide a baseline. IVF-PQ may be included as a separate memory-saving comparison. The dataset subset and policy for handling unjudged query–product results will be documented before evaluation.

## Evaluation

- Recall@k against exact search
- nDCG@10 using ESCI relevance judgments
- Query latency and throughput
- Index build time and memory use
- Results across query-length and multi-requirement groups

## Repository Structure

- `src/` — source code
- `docs/` — abstract and literature survey
- `docs/references/` — research papers or their citations and official links
- `data/` — dataset documentation or approved data files
- `results/` — benchmark outputs
- `reports/` — project reports and review materials

## Status

The project is in the planning stage. No benchmark results are claimed yet.

## References

- Malkov and Yashunin, “Efficient and Robust Approximate Nearest Neighbor Search Using Hierarchical Navigable Small World Graphs.” [arXiv:1603.09320](https://arxiv.org/abs/1603.09320)
- Jégou, Douze, and Schmid, “Product Quantization for Nearest Neighbor Search.” [DOI: 10.1109/TPAMI.2010.57](https://doi.org/10.1109/TPAMI.2010.57)
- Reddy et al., “Shopping Queries Dataset: A Large-Scale ESCI Benchmark for Improving Product Search.” [arXiv:2206.06588](https://arxiv.org/abs/2206.06588)
