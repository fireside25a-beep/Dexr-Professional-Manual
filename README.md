
<!-- ========================================================= -->
<!-- DEXR PROFESSIONAL MANUAL                                  -->
<!-- Complete responsive README for desktop and mobile         -->
<!-- ========================================================= -->

<div align="center">

<a href="https://dexr.lumusmaxima.ai/">
  <img
    src="https://readme-typing-svg.demolab.com?font=monospace&weight=700&size=24&duration=2200&pause=650&color=00E5FF&center=true&vCenter=true&repeat=true&width=850&height=160&lines=%24+booting+DEXR...;%24+loading+NeuroRoute...;%24+initializing+bounded+agents...;%24+checking+approved+tools...;%24+building+verified+state...;%24+running+quine+fixed-point+proof...;%24+validation+passed.;%24+DEXR+ready."
    alt="DEXR animated terminal introduction"
    width="100%"
  />
</a>

# DEXR

### Deterministic · Recursive · Verifiable

**A local-first AI workspace with bounded agents, approval-gated tools, validation, repair, rollback and quine fixed-point verification.**

<br>

[![DEXR Website](https://img.shields.io/badge/DEXR-Official_Website-00D9FF?style=for-the-badge)](https://dexr.lumusmaxima.ai/)
[![LumusMaxima](https://img.shields.io/badge/By-LumusMaxima-071827?style=for-the-badge)](https://lumusmaxima.ai/)
[![Local First](https://img.shields.io/badge/Design-Local_First-00B8D9?style=for-the-badge)](https://dexr.lumusmaxima.ai/)
[![Status](https://img.shields.io/badge/Status-Active_Development-00D9FF?style=for-the-badge)](https://dexr.lumusmaxima.ai/)

</div>

---

<div align="center">


</div>

---

## What is DEXR?

**DEXR** is a local-first AI workspace built around deterministic routing, controlled recursive execution, approved tools, local project state and verifiable build workflows.

The system separates generative assistance from execution authority.

A model may help reason, plan or generate content, but DEXR controls:

- Which policies apply.
- Which tools may run.
- Which workspace may be accessed.
- How deeply agents may recurse.
- How many repair attempts are permitted.
- Which validation gates must pass.
- Whether a candidate may be promoted.
- When rollback is required.

The central principle is:

> **A result is not accepted merely because it was produced. It must pass the required verification gates.**

Projects, logs, reports, state snapshots, manifests and generated artifacts are designed to remain under the user’s control.

---

## Core Principles

<table>
<tr>
<td width="25%" align="center">

### Local-First

Projects and operational state remain on the local machine.

External cloud execution is not required for the core architecture.

</td>
<td width="25%" align="center">

### Deterministic

NeuroRoute applies controlled routing, policy and tool-selection rules.

Equivalent approved inputs are intended to follow the same bounded path.

</td>
<td width="25%" align="center">

### Recursive

Complex work can be divided into smaller specialised tasks.

Recursion depth and repair attempts remain limited.

</td>
<td width="25%" align="center">

### Verifiable

Builds, outputs and reproduced source trees must pass defined verification gates.

Failed candidates cannot be silently promoted.

</td>
</tr>
</table>

---

## High-Level Architecture

```text
USER
 │
 ▼
DEXR INTERFACE
 │
 ▼
PROJECT AND STATE MANAGER
 │
 ▼
NEUROROUTE DETERMINISTIC CORE
 │
 ├── Policy selection
 ├── Route selection
 ├── Tool selection
 ├── Execution boundaries
 └── Validation requirements
 │
 ▼
BOUNDED RECURSIVE AGENT MESH
 │
 ├── Planning
 ├── Task decomposition
 ├── Approved execution
 ├── State recording
 └── Bounded repair
 │
 ▼
VERIFICATION GATES
 │
 ├── Output validation
 ├── Integrity checks
 ├── Build checks
 ├── Test checks
 ├── Reproduction checks
 └── Fixed-point verification
 │
 ▼
RESULTS AND ARTIFACTS
 ├── Logs
 ├── Reports
 ├── Snapshots
 ├── Manifests
 └── Generated files
```

---

## Request Lifecycle

Every accepted request follows a controlled and auditable path.

```text
INPUT RECEIVED
      │
      ▼
ROUTE
NeuroRoute selects applicable policies and execution paths.
      │
      ▼
PLAN
The request is divided into bounded steps.
      │
      ▼
EXECUTE
Only approved tools operate inside the selected workspace.
      │
      ▼
VALIDATE
Outputs are checked against active policies and gates.
      │
      ├── PASS ────────────────────────────────┐
      │                                       │
      └── FAIL                                │
            │                                 │
            ▼                                 │
          REPAIR                              │
      Bounded attempts                        │
            │                                 │
            ▼                                 │
        RE-VALIDATE                           │
            │                                 │
            └─────────────────────────────────┤
                                              ▼
                                           RESPOND
                                  Results, logs and artifacts
```

DEXR does not rely on unlimited autonomous retries.

Repair attempts are bounded, recorded and followed by complete re-validation.

---

## NeuroRoute Deterministic Core

**NeuroRoute** is the deterministic routing engine at the centre of DEXR.

Its responsibilities include:

- Analysing the current request and context.
- Selecting applicable policies.
- Selecting permitted execution paths.
- Choosing approved tools.
- Enforcing workspace boundaries.
- Applying deterministic routing decisions.
- Coordinating deterministic and model-assisted operation.
- Recording routing and execution decisions.
- Preventing unrestricted generated output from becoming automatic authority.

DEXR can perform deterministic operations without requiring a language model.

An optional local model may assist with tasks that need generative reasoning while the surrounding execution pipeline remains controlled by DEXR.

---

## Bounded Recursive Agents

DEXR may decompose a larger request into specialised sub-tasks.

Each agent operates under explicit constraints:

```text
Bounded recursion depth
Bounded execution steps
Bounded repair attempts
Approved tool list
Selected workspace boundary
Validation requirements
Recorded actions and results
```

Recursive execution does not mean unlimited access or unlimited authority.

Every agent remains subject to the same policies, tool approvals and verification requirements.

---

## Approval-Gated Tools

Tools do not execute merely because an agent requests them.

```text
AGENT REQUEST
      │
      ▼
POLICY EVALUATION
      │
      ├── DENIED
      │     └── Action does not execute
      │
      └── APPROVED
            │
            ▼
      BOUNDED EXECUTION
            │
            ▼
      LOGGED AND VALIDATED
```

Tool categories may include:

- Workspace file operations.
- Local shell commands.
- Local Git operations.
- Project search.
- Build utilities.
- Test utilities.
- Validation tools.
- Reporting tools.
- Custom locally configured tools.

Tool availability depends on the active policy and selected workspace.

---

## Local-First Operation

DEXR is designed around local ownership and local execution.

### Local by design

- No required external cloud model.
- No required online account for core operation.
- No mandatory remote project storage.
- Project files remain local.
- Logs and reports remain local.
- Manifests remain local.
- State snapshots remain local.
- Deterministic operation can function without a model.

### Optional local model

A local model runtime may communicate through the loopback interface:

```text
127.0.0.1
::1
localhost
```

The model assists with reasoning or generation.

It does not replace DEXR’s routing, policy, validation or promotion controls.

---

## Quine Self-Reproduction

DEXR includes a quine-oriented source-reproduction workflow.

The objective is not merely to extract or copy files.

A reproduced generation must be checked against the canonical state and must pass the required build, test and integrity checks.

```text
GENERATION 0
Canonical source
      │
      ▼
GENERATION 1
Reproduced source tree
      │
      ▼
BUILD AND TEST
      │
      ▼
GENERATION 2
Reproduced again from the verified generation
      │
      ▼
FIXED-POINT COMPARISON
```

The expected relationship is:

```text
root(gen0) = root(gen1) = root(gen2)
```

A successful proof requires:

```text
Zero missing canonical files
Zero unexpected canonical files
Zero changed canonical bytes
Zero unexpected file-mode changes
Matching canonical generation roots
Successful build and test gates
Successful verification report
```

Reproduction alone is not proof.

---

## Fixed-Point Verification

DEXR compares reproduced generations before permitting promotion.

```text
GENERATION N                     GENERATION N+1
────────────                     ──────────────
Source tree                      Rebuilt source tree
Build                            Build
Tests                            Tests
State root Hₙ                    State root Hₙ₊₁
        │                              │
        └──────────────┬───────────────┘
                       │
                       ▼
                  Hₙ = Hₙ₊₁ ?
                   │         │
                  NO        YES
                   │         │
                   ▼         ▼
            Reject/repair   Record proof
                            and allow
                            promotion review
```

A failed proof cannot silently replace the known-good state.

---

## Promotion and Rollback

Verified candidates follow a controlled promotion path.

```text
CANDIDATE PRODUCED
       │
       ▼
BUILD AND TEST PASSED
       │
       ▼
FIXED POINT VERIFIED
       │
       ▼
SNAPSHOT RECORDED
       │
       ▼
MANIFEST CHECKED
       │
       ▼
AUDIT HASH RECORDED
       │
       ▼
PROMOTION ALLOWED
```

If validation fails:

```text
VALIDATION FAILURE
       │
       ▼
PROMOTION BLOCKED
       │
       ▼
CANDIDATE ISOLATED
       │
       ▼
ROLLBACK TO LAST VERIFIED STATE
       │
       ▼
BOUNDED REPAIR ATTEMPT
       │
       ├── PASS → candidate may return to verification
       │
       └── FAIL → known-good state remains active
```

Promotion and rollback are recorded through state history, manifests and logs.

---

## Verification Gates

DEXR applies layered verification instead of relying on one final test.

1. Input validation.
2. Request classification.
3. Plan validation.
4. Workspace-boundary checks.
5. Tool-policy checks.
6. Execution checks.
7. Output validation.
8. Integrity verification.
9. Build verification.
10. Test verification.
11. Reproduction verification.
12. Fixed-point comparison.
13. Manifest verification.
14. Promotion eligibility.
15. Rollback readiness.
16. Tamper-detection checks.
17. Native target checks.
18. Final attestation.

Failure at a required gate blocks normal promotion.

---

## State Layout

DEXR separates canonical state from operational state.

```text
DEXR STATE
│
├── CONFIGURATION
│   ├── Policies
│   ├── Limits
│   ├── Build settings
│   └── Verification rules
│
├── QUINE REGISTRY
│   ├── Canonical capsules
│   ├── Generation roots
│   ├── Fixed-point proofs
│   └── Promotion records
│
├── AGENT STATE
│   ├── Plans
│   ├── Execution records
│   ├── Tool decisions
│   └── Bounded recursion state
│
├── LOCAL MEMORY
│   ├── Episodic memory
│   ├── Semantic memory
│   ├── Tool cache
│   └── Routing state
│
├── WORKSPACE STATE
│   ├── Versioned files
│   ├── Snapshots
│   ├── Diffs
│   └── Generated artifacts
│
└── AUDIT STATE
    ├── Logs
    ├── Reports
    ├── Manifests
    ├── Hash records
    └── Timestamps
```

Operational data is not automatically treated as canonical source.

---

## Repair Decision Model

DEXR first classifies a failure before selecting a repair path.

```text
FAILURE DETECTED
       │
       ▼
IS IT TRANSIENT?
       │
       ├── YES
       │     │
       │     ▼
       │  BOUNDED RETRY
       │     │
       │     ▼
       │  RE-VALIDATION
       │
       └── NO
             │
             ▼
       CLASSIFY FAILURE
             │
             ├── Drift
             ├── Corruption
             ├── Configuration
             ├── Dependency
             └── Environment
                     │
                     ▼
              SELECT REPAIR
                     │
                     ▼
              VERIFY CANDIDATE
                     │
                     ├── PASS → return to promotion checks
                     └── FAIL → rollback remains active
```

Repair never bypasses the verification gates that rejected the original candidate.

---

## Deterministic Build Flow

```text
CANONICAL SOURCE
      │
      ▼
CONTROLLED BUILD ENVIRONMENT
      │
      ▼
BUILD
      │
      ▼
TEST
      │
      ▼
CREATE CANONICAL MANIFEST
      │
      ▼
HASH CANONICAL FILES
      │
      ▼
REPRODUCE INTO CLEAN DESTINATION
      │
      ▼
REBUILD AND RETEST
      │
      ▼
COMPARE CONTENT AND METADATA
      │
      ├── MISMATCH
      │      └── Reject, rollback or bounded repair
      │
      └── MATCH
             │
             ▼
      FIXED-POINT VERIFICATION
             │
             ▼
      RECORDED PROMOTION
```

---

## Security Boundaries

DEXR uses explicit boundaries rather than assuming generated output is safe.

### Workspace boundary

Tools operate only within the selected workspace and active policy.

### Tool boundary

Only approved tools may execute.

### Recursion boundary

Agent depth, execution steps and repair attempts remain limited.

### Model boundary

Generated model output does not automatically receive execution authority.

### Network boundary

Core local-first operation does not require an external cloud service.

### Promotion boundary

Unverified candidates cannot replace the known-good state.

### Reproduction boundary

Reproduced output remains untrusted until verification succeeds.

### Audit boundary

Important operations produce logs, reports, manifests or recorded state transitions.

---

## Native Build Matrix

DEXR is designed for native build qualification across multiple targets.

| Platform | Architecture | Qualification stage |
|---|---:|---|
| Linux | x86_64 | Primary qualification target |
| Linux | ARM64 | Additional runtime qualification |
| macOS | Apple Silicon / x86_64 | Native packaging and signing path |
| Windows | x86_64 | Native packaging and signing path |
| Android | ARM64 | Planned qualification path |
| iOS | ARM64 | Planned qualification path |

A successful build is not automatically equivalent to a fully tested, signed and publicly released package.

Each platform requires its own runtime testing, packaging, signing and release verification.

---

## Project Guarantees

| Guarantee | Meaning |
|---|---|
| Local-first | Core project state remains under local control |
| Deterministic routing | Policies and execution paths are selected through controlled logic |
| Bounded recursion | Agents cannot recurse without configured limits |
| Approval-gated tools | Tools execute only when permitted |
| Recorded execution | Important operations produce traceable records |
| Fixed-point verification | Reproduced generations must match the canonical root |
| Controlled promotion | Only verified candidates may be promoted |
| Rollback readiness | A known-good state is preserved |
| Tamper evidence | Canonical changes cause verification failure |
| Platform honesty | Build, test and release status remain separate claims |

---

## Repository Scope

This repository hosts the **DEXR Professional Manual** and supporting architecture material.

The documentation covers:

- Installation and startup.
- Workspace organisation.
- Project state.
- NeuroRoute.
- Recursive agents.
- Local model integration.
- Tool approval.
- Validation.
- Bounded repair.
- State snapshots.
- Quine reproduction.
- Fixed-point verification.
- Promotion.
- Rollback.
- Native build qualification.
- Security boundaries.
- Troubleshooting.
- Release limitations.

---

## Current Development Direction

DEXR continues to develop around the following areas:

- Local-first desktop execution.
- Deterministic NeuroRoute control.
- Bounded recursive agents.
- Approval-gated tools.
- Verifiable project state.
- Quine source reproduction.
- Fixed-point comparison.
- Controlled promotion and rollback.
- Native platform qualification.
- Professional technical documentation.
- Expanded local-model compatibility.
- Additional validators and tool interfaces.
- Packaging, signing and release preparation.

---

## Important Release Notice

DEXR remains under active development.

A platform build should not be described as a finished public release until its own native runtime tests, packaging, signing and release qualification are complete.

The architecture, documentation and verification workflow may continue to evolve as qualification progresses.

---

<div align="center">

## Your Machine. Your Model. Your Data.

DEXR is built for people who want AI-assisted work without surrendering their projects, execution flow or verification process to an external black box.

<br>

[![Explore DEXR](https://img.shields.io/badge/Explore-DEXR-00E5FF?style=for-the-badge)](https://dexr.lumusmaxima.ai/)
[![Visit LumusMaxima](https://img.shields.io/badge/Visit-LumusMaxima-071827?style=for-the-badge)](https://lumusmaxima.ai/)

<br>

**Deterministic · Recursive · Verifiable**

<sub>DEXR by LumusMaxima · 2026</sub>

</div>
