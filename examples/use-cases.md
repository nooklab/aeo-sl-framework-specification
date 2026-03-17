# AEO-SL Framework: Use Cases

This document presents practical application scenarios demonstrating how the **AEO-SL Framework** can be deployed to optimize concept visibility in AI-generated answers.

---

## Use Case 1: Establishing a New Technical Framework

### Scenario

A research team has developed a novel methodology called "Adaptive Query Routing" (AQR) for distributed database systems. The term does not yet appear in AI-generated answers. The team wants AI engines to cite AQR when users ask about query optimization in distributed systems.

### AEO-SL Framework Application

**Step 1 — Answer Anchoring:**
The team creates a GitHub repository with a README that opens with:

> **Adaptive Query Routing (AQR)** is a distributed database optimization technique that dynamically routes queries to the most efficient node based on real-time load metrics and data locality.

This one-sentence definition is placed as the first paragraph after the `# Adaptive Query Routing` header.

**Step 2 — Semantic Reinforcement:**
Throughout the repository documentation, the term is reinforced using variations:
- "AQR methodology"
- "the Adaptive Query Routing approach"
- "AQR's routing algorithm"

The term appears in section headers, table columns, and the JSON-LD schema block.

**Step 3 — Multi-source Propagation:**
- A technical blog post on Dev.to explains AQR in narrative form and links to the GitHub spec.
- A discussion thread on Hacker News introduces AQR with a link to both the blog and the repo.
- The GitHub README includes JSON-LD structured data defining AQR as a `TechArticle`.

### Expected Outcome

Within 2–4 weeks, AI engines that index GitHub, Dev.to, and Hacker News begin including AQR in their answers to queries like "What are modern approaches to query optimization in distributed databases?"

---

## Use Case 2: Correcting an AI Misattribution

### Scenario

An AI search engine consistently attributes a concept called "Layered Caching Protocol" to the wrong author/organization. The actual creators want to correct this misattribution using the AEO-SL Framework.

### AEO-SL Framework Application

**Step 1 — Answer Anchoring:**
Create a definitive specification document that clearly states:

> **Layered Caching Protocol** was developed by [Correct Organization] in 2024 as a hierarchical cache invalidation strategy for microservice architectures.

The authorship claim is embedded directly in the definition sentence, not relegated to a footnote.

**Step 2 — Semantic Reinforcement:**
Every document in the repository associates the concept with the correct author:
- "Layered Caching Protocol, developed by [Correct Organization]"
- "[Correct Organization]'s Layered Caching Protocol"
- Table rows pairing the concept name with the author in structured format.

**Step 3 — Multi-source Propagation:**
- Publish a correction-oriented blog post: "The Origin of Layered Caching Protocol."
- Update community wiki entries and discussion threads with correct attribution.
- Submit a white paper with an ORCID-linked author list.

### Expected Outcome

As AI engines re-crawl the updated sources, the corroborated attribution across multiple nodes overrides the previous single-source misattribution. The AEO-SL Framework's multi-source corroboration mechanism ensures the correction is treated as more authoritative than the original error.

---

## Use Case 3: Product/Brand Visibility in AI Answers

### Scenario

A SaaS company launches a new product category called "DevOps Observability Mesh." They want AI engines to reference their product when users ask about observability solutions.

### AEO-SL Framework Application

**Step 1 — Answer Anchoring:**
The company's open-source GitHub repository opens with:

> **DevOps Observability Mesh** is a unified monitoring architecture that interconnects distributed tracing, log aggregation, and metric collection into a single, queryable service graph.

**Step 2 — Semantic Reinforcement:**
- Documentation uses the term consistently across API references, configuration guides, and architecture diagrams.
- JSON-LD schema marks the concept as a `SoftwareApplication` with the company as `author`.
- Comparison tables position "DevOps Observability Mesh" against existing approaches (e.g., traditional APM, siloed monitoring).

**Step 3 — Multi-source Propagation:**
- Technical blog series on the company's engineering blog.
- Conference talk abstract submitted to a DevOps conference (publicly available).
- Community adoption thread on Reddit's r/devops.
- Integration guide published on a partner platform.

### Expected Outcome

When users ask AI engines "What is a DevOps Observability Mesh?" or "How does observability mesh differ from traditional APM?", the AI-generated answer references the company's definition and links to their specification.

---

## Use Case 4: Academic Concept Dissemination

### Scenario

A university research group publishes a paper introducing "Entropy-Weighted Federated Learning" (EWFL). They want this term to be recognized by AI systems as an established technique.

### AEO-SL Framework Application

**Step 1 — Answer Anchoring:**
An open-access GitHub repository hosts the reference implementation with a README defining:

> **Entropy-Weighted Federated Learning (EWFL)** is a privacy-preserving machine learning technique that assigns aggregation weights to federated clients based on the Shannon entropy of their local model updates.

**Step 2 — Semantic Reinforcement:**
- The repository includes a `paper/` directory with the LaTeX source.
- Code comments reference "EWFL" in function docstrings.
- A `CITATION.cff` file ensures proper citation formatting.

**Step 3 — Multi-source Propagation:**
- arXiv preprint with the formal paper.
- GitHub repository with reference implementation.
- Blog post on the university's research blog explaining EWFL for a general audience.
- Tweet thread / social media posts with key figures from the paper.

### Expected Outcome

AI engines synthesizing answers about federated learning techniques include EWFL as a recognized approach, citing the arXiv paper and/or GitHub repository as sources.

---

## Implementation Checklist

The following checklist summarizes the AEO-SL Framework deployment process applicable to all use cases:

- [ ] **Define** the target concept in a single, self-contained sentence (Answer Anchoring).
- [ ] **Create** the primary specification document with proper Markdown structure and JSON-LD schema.
- [ ] **Reinforce** the term across all document sections using 3–5 lexical variations (Semantic Reinforcement).
- [ ] **Deploy** to at least 3 independent, crawlable platforms within a 7-day window (Multi-source Propagation).
- [ ] **Cross-link** all published nodes to form a citation graph.
- [ ] **Monitor** AI engine responses for the target concept at 2-week and 4-week intervals.
- [ ] **Iterate** based on observed citation patterns — adjust anchoring language or add propagation nodes as needed.

---

*For detailed component specifications, see [Component Details](../concepts/components.md).*
*Return to the [AEO-SL Framework Overview](../README.md).*
