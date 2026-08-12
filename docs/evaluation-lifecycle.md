# Evaluation lifecycle

This document defines the evaluation lifecycle used by Multilingual Evaluation Lab.

The goal is to make each evaluation reproducible, reviewable, and appropriately bounded. An evaluation should produce evidence for a specific question, not a general claim about a model, language, or multilingual AI system.

A guiding principle is:

**scope → evidence → allowed claim**

The scope determines what evidence must be collected. The evidence determines what claims the evaluation can reasonably support.

## 1. Define the evaluation question

Begin with a specific engineering or research question.

The question should identify the behavior being investigated and should be narrow enough to evaluate with a defined dataset, configuration, and judgment process.

Example:

> How reliably does a selected retrieval system return relevant Finnish passages for the queries in a bounded test set?

The evaluation question is recorded before results are generated.

## 2. Define the scope

Document the boundaries of the evaluation.

The scope should identify:

- task
- language or languages
- dataset or test cases
- system or model configuration
- retrieval or generation settings
- evaluator types
- metrics or judgment criteria
- known exclusions

Anything outside these boundaries is outside the evaluation's claim scope.

## 3. Define the evidence plan

Specify what evidence is needed to answer the evaluation question.

Evidence may include:

- automated metrics
- retrieved results
- expected-answer or relevance judgments
- human-review records
- evaluator outputs
- observed failure cases
- error classifications

The evidence plan should be defined before interpreting results.

## 4. Execute the evaluation

Run the evaluation using the documented configuration.

Where practical, record:

- input data
- configuration
- model or retrieval settings
- evaluator version
- scoring criteria
- generated outputs
- timestamps or run identifiers

Evaluation definitions should remain separate from evaluation results so that the same specification can be rerun.

## 5. Review and judge the evidence

Evaluate the collected outputs using the criteria defined in the evaluation specification.

Automated metrics and human judgments serve different purposes and should not be treated as interchangeable.

Human review should be used where relevance, meaning, linguistic quality, or contextual interpretation cannot be adequately represented by an automated metric alone.

## 6. Analyze errors

Record meaningful failure cases rather than reporting only aggregate scores.

Error analysis may identify:

- retrieval failures
- relevance errors
- language-specific failures
- ambiguous test cases
- evaluator disagreement
- dataset limitations
- configuration-related failures

Error categories may evolve as evidence accumulates, but changes to the classification scheme should be documented.

## 7. Determine the allowed claim

Conclusions must remain within the scope supported by the collected evidence.

An evaluation may support a claim about:

- the tested system
- the tested configuration
- the defined dataset
- the evaluated language or language setting
- the observed behavior under those conditions

It should not automatically support claims about:

- all models
- all datasets
- an entire language
- all speakers or language varieties
- multilingual AI systems generally

A successful result in one language does not establish equivalent performance in another.

## 8. Record limitations

Limitations are part of the evaluation result.

Document factors that constrain interpretation, including:

- dataset size or composition
- language coverage
- evaluator coverage
- model or system coverage
- metric limitations
- uncertainty or disagreement
- untested conditions

Limitations should directly inform the allowed claim.

## Lifecycle output

A completed evaluation should leave enough evidence for another reviewer to understand:

1. what question was asked
2. what was tested
3. what evidence was collected
4. how the evidence was judged
5. what failures were observed
6. what limitations apply
7. what claim the evidence can reasonably support

The lifecycle is complete only when the conclusion can be traced back through the evidence to the original evaluation scope.