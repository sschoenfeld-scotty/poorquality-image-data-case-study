# Material Inflection Points

This log captures architectural decisions that materially changed the operating system. It is not a batch diary.

| Inflection point | Evidence or constraint | Decision | Why it changed the system |
| --- | --- | --- | --- |
| Visual extraction proved feasible | Early batches produced useful structured records | Continue with direct visual review as the evidentiary authority | Feasibility was established without treating automated text extraction as canonical truth |
| Duplicate source material entered normal processing | Repeated images and copy-marked files could cause repeated evidence review | Govern source eligibility before extraction | Record quality controls were insufficient if the source boundary itself was polluted |
| One canonical mutable master became necessary | Intermediate exports could create competing authorities | Use one persistent working master for committed data | The workflow needed one source of truth for writes, recovery, and reconciliation |
| Exact-name identity rules were formalized | Similar names and repeated appearances created merge risk | Use minimal normalization and exact-name matching only | Conservative identity evidence was safer than plausible but unsupported fuzzy resolution |
| Blank-field-only enrichment was introduced | Existing records could contain supported data that should not be overwritten | Enrich only supported blank fields | Preservation of prior populated values reduced mutation risk |
| Durable execution state became mandatory | Long-running threads could stop after review, reconciliation, or mutation | Move operational continuity outside conversation history | A new session had to reconstruct the verified next action without restarting completed work |
| Checkpoints became reconstructable | Simple completion markers could not prove what had actually been verified | Require state to preserve scope, evidence, reconciliation, writes, exceptions, and next action | Recovery needed evidence, not status labels |
| Attempted-write recovery was added | An interruption could make write status uncertain | Read the exact destination before replaying any uncertain mutation | Read-before-replay reduced duplicate writes and avoided blind recovery |
| Source chronology became part of completion | Finishing one active source area did not prove that restored historical material was exhausted | Require stable chronological source exhaustion before final reconciliation | Local completion could otherwise create a false project completion state |
| Instructions became a control plane | Repeated failures exposed missing source, identity, recovery, and mutation rules | Encode recurring judgment into explicit project instructions | The prompt evolved from a request into an operating contract |
| A compression audit rejected weakened instructions | Shortening the operating instructions weakened recovery and trace protections | Reject the compressed version and restore the missing controls | Brevity was not allowed to reduce recoverability or evidence quality |
| Source-grounded reconstruction superseded an earlier aggregate result | Direct review produced 376 unique readable people where earlier controls recorded 220 | Preserve the historical result as variance evidence and let verified source evidence supersede it | The system had to allow reality to overturn its own prior answer |
| One-check reconciliation simplified routine execution | Repeating verified zero-match checks added work without adding evidence | Require one fresh live exact-name check for each unmatched verified spelling | More checking was not automatically more integrity |
| Continuity gates were split by context | Full recovery checks were useful after interruption but redundant inside one verified execution chain | Use a full gate after interruption and a lighter same-chain gate during continuous execution | Governance became proportional to the actual uncertainty |
| Model configuration was pressure tested | A mature governed workflow experienced friction under more complex reasoning and later completed one clean Instant batch in about 11 minutes | Treat model choice as workload-dependent rather than assuming maximum reasoning is always better | The architecture had absorbed more decision logic, reducing the need for open-ended execution reasoning |
| Additional execution environments remained optional | The workflow continued to operate safely inside Chat after hardening | Retain Chat as the minimum sufficient execution environment through completion | Architectural complexity was added only when evidence required it |
| Final reconciliation followed proven source exhaustion | All eligible source had been processed and durable state was complete | Run the final duplicate sweep, reconcile totals, replace the final export, and verify it | Closure was evidence-driven rather than declared from convenience |

## Decision Pattern

Across these changes, the same pattern repeated.

1. A real execution failure exposed a weak assumption.
2. The failure was diagnosed at the system level rather than patched only at the local step.
3. A new control was introduced.
4. The control was tested in later execution.
5. Once the evidence threshold was met, repeated checking was reduced rather than preserved as ritual.

The project became more autonomous because the boundaries became more explicit, not because human accountability disappeared.
