<>Markdown
#PropertyIQ Team Plan
##Requirement Reviewed
The team reviewed requirements.txt for the PropertyIQ project.

##Project Objective
PropertyIQ is a real-estate property-search and deal analysis assistant. The app will help first-time buyers match listings to their criteria using RAG over listing and neighborhood data. Later phases will add mortgage calculation, comparable-sales analysis, buyer memory, fair-housing guardrails, caching, and observability.

## User Persona

David and Elena Torres are first-time home buyers. They are looking for:

- 3-bedroom homes
- Under $450K
- Good school district
- Clear affordability numbers
- Comparable-sales/deal analysis
- No repeated listings they already rejected

## Week 1 Goal

Build a basic RAG-based prototype that can answer:

> Find 3-bed homes under $450K near good schools in Maple Heights.

## Team Ownership Model

The team is following a shared ownership model. All team members will contribute across the core areas of the application instead of assigning each feature to only one person.

Core areas include:

- Prompt design and RAG retrieval
- Listing and neighborhood data preparation
- Tools and MCP integration
- Buyer memory and rejected-listing handling
- Fair-housing guardrails and caching
- Observability and UI/demo readiness

## Collaboration Approach

Although ownership is shared, the team will coordinate work through feature branches and pull requests. Each change should be reviewed before merging into `main`.

Recommended branch pattern:

```text
main
feature/week1-setup
feature/rag-ingestion
feature/gradio-ui
feature/guardrails
feature/memory
feature/tools-mcp

# Tech Stack
************

| Layer           | Tool                  |
| --------------- | --------------------- |
| Language        | Python                |
| UI              | Gradio                |
| Data format     | JSON                  |
| Vector Store    | ChromaDB              |
| Embeddings      | Sentence Transformers |
| Version Control | GitHub                |

Future phases may add MCP tools, mortgage calculator tools, buyer memory, caching, observability, and evaluation scripts.