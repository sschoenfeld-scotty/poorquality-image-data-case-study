# Architecture

This directory documents the operating architecture that emerged from repeated execution failures and recovery work.

- [Mature Batch Workflow](mature-batch-workflow.md) shows the controlled execution path from fixed source scope through durable closure.
- [Interruption Recovery Model](interruption-recovery-model.md) shows how the system resumed safely without blindly replaying completed work.

These documents describe the public architecture and control logic. They intentionally do not publish the complete internal execution instructions.
