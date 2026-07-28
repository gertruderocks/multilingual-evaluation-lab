# Multilingual Benchmark Explorer

> Exploring how multilingual AI systems represent, retrieve, evaluate, and transfer meaning across language families, language contact zones, Indigenous languages, national minority languages, and low-resource language communities.

---

# Why this project?

Modern AI systems must work across languages that differ in morphology, writing systems, available training data, historical relationships, and cultural context.

This repository explores multilingual AI through practical experiments in tokenization, embeddings, retrieval, Retrieval-Augmented Generation (RAG), evaluation, and multilingual NLP.

The project begins with small, reproducible benchmarks in a limited set of anchor languages. Additional languages are introduced selectively when they help answer a specific AI engineering or evaluation question.

The goal is to build a deeper understanding of multilingual AI while developing practical engineering skills relevant to modern AI systems.

---

# Current implementation scope

The first implemented benchmark is a small strict-RAG groundedness evaluation in English and Finnish.

This initial benchmark is designed to test the repository's data model, evaluation workflow, language-level reporting, and distinction between human-reviewed labels and automated evaluator judgments.

The broader language inventory is a structured research map. Inclusion in the inventory does not mean that every language is under active experimentation or will receive equal coverage. The project will expand selectively after the initial evaluation workflow is working reliably.

---
# Research questions

- How well do multilingual AI systems transfer across related languages?
- How do morphology and writing systems influence tokenization and embeddings?
- How does language contact influence multilingual retrieval?
- How should multilingual AI systems be evaluated beyond benchmark scores?
- Which multilingual architectures best support low-resource, Indigenous, and national minority languages?
- How can comparative multilingual experiments improve our understanding of modern AI systems?

---

# Core topics

- Tokenization
- Embeddings
- Morphology
- Information Retrieval
- Retrieval-Augmented Generation (RAG)
- Evaluation
- Multilingual NLP
- Semantic Search
- Cross-lingual Transfer
- Language Contact
- Low-resource NLP
- AI Safety
- Vector Databases
- Benchmark Design

---

# Language coverage

The current implemented benchmark begins with English and Finnish.

The broader research inventory includes languages from several families and contact settings that may support future experiments:

- Uralic
- Germanic
- Slavic
- Baltic
- Turkic
- Kartvelian
- Iranian
- Northeast Caucasian

Languages are added to active experiments only when they support a defined evaluation question.

The authoritative language inventory is maintained in:

- `docs/language-families.md`

Individual AI engineering language profiles are located in:

```text
docs/languages/
```

---

# Comparative methodology

Rather than comparing languages at random, experiments are designed to investigate specific multilingual AI engineering questions.

Potential comparisons include:

| Comparison | Why it matters |
|------------|----------------|
| Finnish ↔ Estonian | Closely related Finnic languages |
| Finnish ↔ Meänkieli | Closely related Finnic languages shaped by different national and sociolinguistic histories |
| Finnish ↔ Russian | Neighboring countries with different language families, writing systems, and centuries of language contact |
| North Sámi ↔ Norwegian | Indigenous language technologies and multilingual public services |
| Dutch ↔ German | Closely related West Germanic languages |
| Russian ↔ Ukrainian | Closely related East Slavic languages |
| Estonian ↔ German | Historical language contact and the development of written Estonian |
| Estonian ↔ Russian | Language contact across Finnic and Slavic languages |
| Azerbaijani ↔ Turkish | Closely related Oghuz Turkic languages |
| Azerbaijani ↔ Persian | Cross-border multilingual communities and language contact |
| Georgian ↔ Armenian | Neighboring languages from different language families |
| Erzya ↔ Finnish | Uralic morphology and low-resource NLP |

Additional comparative methodologies are documented in:

- `docs/comparative-methodology.md`

---

# Documentation

The repository is organized around a set of complementary documents.

| Document | Purpose |
|----------|---------|
| `language-families.md` | Authoritative language inventory |
| `language-contact.md` | Historical and sociolinguistic relationships |
| `comparative-methodology.md` | Experimental design philosophy |
| `tokenization.md` | Tokenization concepts |
| `embeddings.md` | Multilingual embeddings |
| `retrieval.md` | Information retrieval |
| `evaluation.md` | Evaluation strategies |
| `languages/README.md` | Language profile template |

Together, these documents provide the conceptual foundation for the repository while individual language profiles apply these ideas to specific languages.

---

# Repository structure

```text
docs/
│
├── language-families.md
├── language-contact.md
├── comparative-methodology.md
├── tokenization.md
├── morphology.md
├── embeddings.md
├── retrieval.md
├── retrieval-augmented-generation.md
├── evaluation.md
│
├── languages/
│   ├── README.md
│   ├── finnish.md
│   ├── estonian.md
│   ├── dutch.md
│   ├── russian.md
│   └── ...
│
└── adr/

experiments/

visualizations/

blog/
```

---

# Long-term vision

This repository documents my development of multilingual AI evaluation skills through small, reproducible experiments, comparative analysis, and documented system-design decisions.

The long-term goal is to understand how AI systems represent, retrieve, and evaluate meaning across languages while building practical experience with evaluation pipelines, multilingual retrieval, RAG, and language-level reporting.

The project will expand incrementally from a small implemented benchmark. It emphasizes reproducibility, transparent evidence, thoughtful documentation, and evaluation practices that make uneven performance across languages visible.