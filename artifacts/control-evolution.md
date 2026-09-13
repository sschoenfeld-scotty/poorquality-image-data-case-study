# Control Evolution

The operating instructions did not begin as a finished architecture.

They evolved because live execution exposed assumptions that were missing, weak, or too expensive to leave implicit.

This public artifact shows the categories of control that emerged without publishing the complete internal execution prompt.

## Stage 1

### Basic extraction request

The initial workflow centered on reading photographed records and producing structured data.

The early design assumed that strong extraction logic would be enough.

Execution showed that this was incomplete.

## Stage 2

### Source governance

Duplicate source material and copy-marked files could cause repeated evidence review.

The instructions added source eligibility rules, exclusion logic, chronology, and source-boundary controls.

The governing lesson became

> **Source governance before record governance.**

## Stage 3

### Conservative identity rules

Repeated names, similar names, and multiple exact-name rows created identity risk.

The instructions formalized minimal normalization, exact-name matching, ambiguity preservation, and blank-field-only enrichment.

The workflow was designed to reward restraint rather than plausible completion.

## Stage 4

### Canonical data authority

Intermediate outputs could not remain competing authorities.

One persistent working master became the sole mutable authority for committed structured data.

This made later reconciliation, write recovery, and final export inspectable against one canonical surface.

## Stage 5

### Durable execution state

Conversation continuity proved insufficient for long-running work.

The instructions added reconstructable checkpoints that preserved source scope, verified records, reconciliation results, planned writes, exceptions, next action, and mutation status.

The control moved from remembering the conversation to reconstructing operational truth.

## Stage 6

### Mutation safety

Writes were separated from review and reconciliation.

The mature sequence became

1. review source
2. reconcile against the live master
3. checkpoint the planned mutation
4. apply the supported write once
5. read the exact destination back

Uncertain writes used read-before-replay recovery.

This reduced the risk that recovery itself would corrupt the data.

## Stage 7

### Continuity and sufficient checking

Early controls leaned toward repeated verification because repetition felt safer.

Later execution showed that repeated checks could add work and make state harder to reason about after the required evidence threshold had already been met.

The instructions introduced one-check reconciliation and different continuity gates for interrupted sessions versus uninterrupted verified execution chains.

The lesson was not fewer controls.

It was controls proportional to uncertainty.

## Stage 8

### Operating contract

By the mature stage, the instructions governed source eligibility, evidence authority, identity, enrichment, continuity, recovery, mutation, readback, exceptions, source exhaustion, stop conditions, and final closure.

A later attempt to compress those instructions weakened important recovery and trace protections. The compressed version was rejected after audit and the missing safeguards were restored.

> **At that point, the prompt was no longer a request. It had become a tested operating contract.**

## What This Evolution Shows

The workflow did not become reliable because the prompt became longer.

It became more reliable because recurring judgment was moved into inspectable rules and controls only when execution evidence justified the change.

The same discipline later allowed routine execution to become simpler.

Complexity was absorbed by the architecture so the executor needed less improvisation.
