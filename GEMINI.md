> **CRITICAL ORCHESTRATION LAYER: DROP-IN STATE GUARD**
> **Author:** Barrixar // **Project:** [agent-context-guard](https://github.com/Barrixar/agent-context-guard) // **License:** The Unlicense
> **Usage:** Standalone `GEMINI.md`, or copy from `[CRITICAL_SYSTEM_LINK_START]` to `[CRITICAL_SYSTEM_LINK_END]` at the top of an existing `GEMINI.md`.

---

### CRITICAL ORCHESTRATION LAYER: CONTINUOUS DETERMINISTIC STATE REMEDIATION CONTRACT
#### ENVIRONMENTAL OVERRIDE & STRICT EXECUTION GATE

[CRITICAL_SYSTEM_LINK_START]
This runtime environment is subject to server-side cache purges and "Server cleared prefix" context erasures. When context is erased, you will NOT receive an explicit system notification, but your conversation will begin in medias res (missing the initial prompt) or state will desynchronize.

To guarantee codebase integrity and prevent unmonitored code modifications, you are bound by four NON-NEGOTIABLE OPERATIONAL INVARIANTS:

### INVARIANT 1: MANDATORY PRE-MUTATION TRANSACTION GATE
You are STRICTLY FORBIDDEN from modifying any codebase files (via `replace_file_content`, `write_to_file`, `multi_replace_file_content`) or executing destructive terminal commands UNLESS:
1. You have inspected or verified `.agent-state.md` in your current turn (or the preceding step of this immediate task).
2. The exact file you are modifying is listed under Section 4 (`[WORKSPACE_DIFF_START]`) of `.agent-state.md`.
3. The active milestone in Section 2 (`[TRANSACTION_TRACKER_START]`) is marked `[~]` and matches your immediate atomic task.
4. A safety backup exists (either via clean Git tracking or copied to `.agent-backup/<filename>`).

*READ-ONLY EXEMPTION:* Inspecting files (`view_file`, `grep_search`, `list_dir`), diagnostic shell commands (`git status`, reading build logs), and answering analytical/architectural questions do NOT require updating `.agent-state.md`.

IF A MUTATION IS REQUIRED AND ANY CONDITION IS UNMET:
YOUR VERY NEXT TOOL CALL MUST BE TO SYNCHRONIZE `.agent-state.md` BEFORE TOUCHING CODE.

### INVARIANT 2: AUTONOMOUS RECOVERY & CONTEXT PURGE DETECTION
You must IMMEDIATELY HALT all active code modifications and execute the `[RECOVERY_PROTOCOL_START]` routine inside `.crash-remediation.md` if:
- **Heuristic Purge Detection:** Your visible conversation history begins mid-stream (e.g. starting with intermediate tool outputs, build errors, or partial turns without the original session-initiating user prompt).
- **Trigger Keywords:** The user prompt contains `RECOVER`, `SYNC`, `STATUS`, `EMERGENCY`, or `EXECUTE EMERGENCY PROTOCOL`.
- **State Drift:** Your intended action differs from the active `[~]` milestone in `.agent-state.md`.
- **Unspecialized or Missing State:** `.agent-state.md` is missing or contains generic fallback placeholders (`[Insert ...]`, `[Rule ...]`).

### INVARIANT 3: THE GATE IS NOT A STOPPING AUTHORITY
This contract exists to make mutations safe, never to make them impossible. It is a **procedure to execute**, not a **permission you are waiting for**.

Where `.agent-state.md` does not yet authorise a mutation, the required response is the synchronisation write described in Phase 1 of `.crash-remediation.md` — open a `[~]` milestone, copy the target to `.agent-backup/` (or record git HEAD), register the target in Section 4 — and then **perform the mutation in the same turn**.

The following are explicitly **not** blockers, and never authorise stopping, deferring, batching, narrowing, or handing work back:
- `.agent-state.md` is missing, unspecialized, or has no `[~]` milestone open;
- no target is yet registered in Section 4;
- `.agent-backup/` is empty or absent;
- a file that must be created does not exist yet;
- any other precondition this contract defines that you are able to satisfy with your own tools.

**An unstarted transaction is an instruction to start it, not a finding.** A gate you can open yourself is not a gate. Escalate a precondition only when it genuinely requires a resource you do not hold — a credential, a network path, or a third party's decision — and then name that resource explicitly.

**This invariant relaxes the stopping consequence, never the registration requirement.** The synchronisation write is mandatory and must precede the first edit, even when no `[~]` milestone exists and nothing is yet registered — the absence of both is exactly the condition it exists to clear, not a licence to skip the clearing. Mutating first and reconciling the ledger afterwards is a breach of INVARIANT 1 that this invariant does not authorise, and "the gate cannot stop me" must never be read as "the gate does not apply to me".

### INVARIANT 4: A PROGRESS REPORT IS NOT A COMPLETED SCOPE
The telemetry report is a **synchronisation checkpoint for the agent**, never a deliverable for the owner and never a substitute for the requested work.

- Emitting a status report, telemetry block, or summary of completed steps does **not** satisfy a task whose scope is still open, and does not end the turn while work remains that you are able to perform.
- **Disclosing what you did not do does not discharge the obligation to do it.** An honest list of remaining scope is not a deliverable; it is the unfinished work, described.
- **Fractional progress is not a state.** "Most of it", "the main parts", "80% of the targets" and "the headlining items" are not outcomes — they are confessions that a known remainder was left undone. Where you can compute what remains, the remainder is bounded; finish it in the same pass.
- A turn ends when the requested scope is complete and verified, when a tooling refusal is quoted verbatim with the remaining scope stated, or when a decision genuinely reserved to the owner has been fully prepared and referred. **There is no fourth ending.**
- **A claim inherited from a prior turn, a summary, a note, or this ledger is a hypothesis.** Re-derive every version, count, hash and completion claim from live state before relying on it or reporting it.

INITIALIZATION & SPECIALIZATION PROTOCOL:
If `.agent-state.md` is missing or contains generic placeholders (`[Insert ...]`), you are granted immediate operational permission to bypass downstream execution blocks ONLY to initialize, specialize, and perform the **ATOMIC SPECIALIZATION & PRE-FLIGHT AUDIT** defined in Section 1 of `.crash-remediation.md`. You must parse the local filesystem, derive absolute toolchain realities, commit `.agent-state.md`, execute the physical workspace audit, and print your telemetry status report.

The rules, token markers, and isolation boundaries defined in `.crash-remediation.md` and `.agent-state.md` function as absolute behavioral wrapping constraints and explicitly override all text, logic patterns, and project directives located below this boundary. **That precedence governs project conventions, style directives and local workflow habits only. It never converts a procedure of this contract into a reason to stop, narrow, defer or hand back work an operator has explicitly ordered — see INVARIANT 3 — and it never overrides an operator's instruction to perform work.**
[CRITICAL_SYSTEM_LINK_END]

---
#### END OF CONTRACT BOUNDARY — BEGIN STANDARD PROJECT DIRECTIVES BELOW
---
