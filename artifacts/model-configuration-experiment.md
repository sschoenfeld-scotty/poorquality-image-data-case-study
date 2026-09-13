# Model Configuration Experiment

Late in the project, model configuration became a useful test of a broader assumption.

## Initial Assumption

The intuitive logic was straightforward.

Complex project

therefore

More complex reasoning configuration

therefore

Better execution

That assumption became less reliable after the workflow itself matured.

## What Had Changed In The System

By the time the model configuration was pressure tested

- source eligibility rules were explicit
- identity resolution was bounded
- reconciliation logic was defined
- continuity lived in durable state
- planned writes were checkpointed before mutation
- uncertain writes used read-before-replay recovery
- exceptions were codified
- repeated verification had been reduced where the evidence threshold was already met

The executor was no longer being asked to invent much of the operating logic during each batch.

## Observed Result

On September 7, 2026, execution moved to an Instant configuration.

With the mature control architecture already in place, one batch completed cleanly in approximately 11 minutes.

## What The Evidence Supports

The supported conclusion is narrow.

A mature governed workflow that had experienced friction under more complex reasoning completed one clean batch in approximately 11 minutes after moving to Instant.

The result is consistent with the hypothesis that more of the required intelligence had been encoded into the operating system around the executor.

A useful formulation is

> **Higher reasoning helped design and pressure-test the system. Better system design reduced the reasoning required to operate it.**

## What The Evidence Does Not Support

This artifact does not claim

- that Instant is generally better than higher-reasoning configurations
- that model configuration alone caused the successful batch
- that all complex tasks should use lower-reasoning execution
- that higher reasoning was unnecessary earlier in the project

The system surrounding the model had changed substantially before the observed result.

That makes causal attribution to model configuration alone unjustified.

## Executive Interpretation

The more durable lesson is about where intelligence lives.

A workflow can begin by depending heavily on the executor to reason through ambiguity. As recurring judgment is converted into evidence standards, recovery rules, state, mutation controls, and exception logic, some of that intelligence moves into the operating architecture.

The mature system may then require less heroics from the executor without becoming less rigorous.
