# Multilingual Evaluation Lab

A practical evaluation project for studying how multilingual AI systems retrieve, represent, and transfer meaning across languages.

The v1 case study focuses on Finnish retrieval evaluation, with a small comparison set of additional languages used only where they support a defined evaluation question.

## Why this project?

Multilingual AI systems operate across languages that differ in morphology, writing systems, available training data, historical relationships, and cultural context.

This project develops small, reproducible evaluations for investigating those differences while practicing evaluation design, retrieval, error analysis, structured reporting, and multilingual NLP.

A working evaluation principle is:

**Scope → evidence → allowed claim**

Each evaluation should make clear:

- what is being tested
- what evidence was collected
- how results were judged
- what limitations apply
- what conclusions the evidence can reasonably support

## v1 scope

The first implementation focuses on a bounded Finnish retrieval evaluation.

The v1 language set is:

- Finnish
- Estonian
- North Sámi
- Swedish
- Norwegian
- Dutch
- Russian

Finnish is the primary case-study language. The other languages are comparison languages, not a commitment to build a complete benchmark suite for each one.

A language is included in an active evaluation only when it serves a defined evaluation question and appropriate data can be created or sourced responsibly.

## v1 goals

- define a reproducible multilingual retrieval evaluation
- separate evaluation definitions from evaluation results
- combine automated metrics with human-reviewed judgments
- record error cases and limitations
- produce machine-readable evaluation artifacts
- make claims that remain within the documented evaluation scope

## Current focus

The current implementation is intentionally narrow.

Primary areas of work include:

- multilingual retrieval evaluation
- Finnish as the primary case study
- human-reviewed and automated judgments
- error analysis
- machine-readable evaluation definitions and results
- reproducible evaluation design
- explicit limitations and claim boundaries

## Evaluation approach

Evaluations should be designed around a specific engineering or research question rather than around broad language coverage.

A typical evaluation should document:

1. the evaluation question
2. the scope and language coverage
3. the dataset or examples used
4. the retrieval or model configuration
5. the metrics and evaluator types
6. human-review criteria where applicable
7. observed failure cases
8. limitations
9. conclusions supported by the available evidence

Evaluation definitions and evaluation results should remain separate so that experiments can be rerun, compared, and reviewed without changing the original evaluation specification.

## Language coverage

Finnish is the primary v1 case-study language.

The comparison set includes:

- Estonian
- North Sámi
- Swedish
- Norwegian
- Dutch
- Russian

These languages provide useful contrasts in morphology, language family, resource availability, regional context, and multilingual model behavior.

They are not all active benchmark targets in v1.

Language-specific notes are maintained in [`docs/languages/`](docs/languages/).

## Comparative methodology

Comparisons are designed around specific multilingual AI questions rather than around language pairs chosen only because they are historically or geographically related.

Useful comparison dimensions may include:

- related languages with different resource levels
- languages with different morphological characteristics
- majority-language and minority-language settings
- differences in retrieval behavior
- differences in error patterns
- differences in evaluator confidence or coverage

The goal is not to rank languages. The goal is to understand when and why an evaluation workflow behaves differently across language settings.

See [`docs/comparative-methodology.md`](docs/comparative-methodology.md) for the developing comparative framework.

## Evaluation artifacts

The project will use structured artifacts so that evaluation decisions and results can be inspected independently.

Planned artifact types include:

- evaluation definitions
- query or test-case records
- expected-answer or relevance judgments
- evaluator outputs
- human-review records
- error classifications
- result summaries
- limitation records
- evaluation-scope and claim records

JSON will be used where machine-readable records are useful.

## Documentation

Core documentation will focus on the evaluation system rather than on maintaining a broad catalog of multilingual AI topics.

Current and planned documentation includes:

- [`docs/evaluation.md`](docs/evaluation.md) — evaluation concepts and strategy
- [`docs/comparative-methodology.md`](docs/comparative-methodology.md) — comparative evaluation principles
- [`docs/retrieval.md`](docs/retrieval.md) — retrieval concepts relevant to the case study
- [`docs/languages/`](docs/languages/) — language-specific notes for the v1 comparison set

Planned v1 documentation includes:

- `docs/architecture.md`
- `docs/evaluation-lifecycle.md`
- `docs/evaluator-types.md`
- a Finnish retrieval case-study document
- machine-readable evaluation definitions and results

Some existing exploratory documents may be revised, archived, or removed as the repository is narrowed around the v1 evaluation workflow.

## Future investigation areas

Possible extensions after v1 include:

- cross-lingual retrieval
- multilingual embeddings
- tokenization and morphology
- retrieval-augmented generation
- evaluation in lower-resource language settings
- prompt regression testing

These are future directions, not v1 commitments.

## Reproducibility

The project aims to make evaluation work understandable and repeatable.

Where possible, each experiment should record:

- input data
- configuration
- model or retrieval settings
- evaluator version
- scoring criteria
- human-review criteria
- result artifacts
- known limitations

Changes to evaluation definitions should be versioned rather than silently replacing earlier specifications.

## Limitations

This project is intentionally small.

Results from a limited language set, dataset, model, or evaluator should not be generalized to multilingual AI systems as a whole.

A successful result in one language does not establish equivalent performance in another language.

Automated metrics should not be treated as substitutes for human review when meaning, relevance, or linguistic quality requires interpretation.

The project therefore treats limitations as part of the evaluation result rather than as an afterthought.

## Long-term vision

Multilingual Evaluation Lab will develop incrementally through small, reproducible experiments.

The long-term goal is to build practical experience with multilingual AI evaluation while documenting how scope, evidence, evaluator design, and language characteristics affect the conclusions that can responsibly be drawn from an experiment.

The project emphasizes transparent evidence, reproducibility, explicit limitations, and careful interpretation of uneven performance across languages.