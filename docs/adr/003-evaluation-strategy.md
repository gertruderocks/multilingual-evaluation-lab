# ADR 003: Multilingual evaluation strategy

## Status

Accepted

## Context

The Multilingual Benchmark Explorer needs a consistent way to evaluate multilingual AI systems across languages, components, and end-to-end workflows.

A single aggregate score can hide serious failures in individual languages, language groups, or evaluation categories. The project therefore needs an evaluation strategy that makes uneven performance visible and separates human judgment from automated evaluation.

## Decision

The project will evaluate the whole system, not only the underlying model.

Evaluation will be organized around three dimensions:

- Capability
- Safety
- Evidence quality

The evaluation approach will combine:

- Deterministic component tests
- Scenario-based system evaluations
- Human-reviewed labels
- Automated evaluator judgments

Human labels and automated evaluator results will be stored separately so that evaluator agreement and disagreement can be measured.

Results will be reported by language and evaluation category. The project will also track worst-language performance, severe failures, and other subgroup results rather than relying only on overall averages.

The first implemented benchmark will be a small strict-RAG groundedness benchmark in English and Finnish.

Initial groundedness evaluation will track:

- Supported claims
- Unsupported claims
- Contradicted claims
- Missing or insufficient evidence
- Citation quality
- Latency and cost when applicable

## Consequences

This strategy creates a reusable foundation for future multilingual benchmarks.

It also requires more detailed test data, language-specific reporting, and careful distinction between reference labels and automated judgments.

The initial benchmark will remain deliberately small so that the data model and evaluation workflow can be tested before the project expands to more languages and metrics.