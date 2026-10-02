# Stamatis-Christos Saridakis

### Systems Engineer · Independent Researcher

I design and build reliability-focused systems across **agentic AI, distributed systems, databases, transactional platforms, runtime assurance, and verifiable infrastructure**.

A recurring question connects much of my work:

> **How do we make increasingly autonomous software remain correct, auditable, recoverable, and controllable across multi-step execution?**

My projects explore this problem from several directions: agent execution contracts, runtime policy enforcement, distributed databases, deterministic transaction processing, cryptographic evidence systems, symbolic verification, recovery semantics, and high-assurance infrastructure.

---

## 📄 Published Research

### AARC — A Machine-Verifiable Audit and Reliability Contract for Tool-Using AI Agents

AARC defines a machine-verifiable execution contract for tool-using AI agents based on externally observable runtime evidence rather than hidden chain-of-thought.

It focuses on:

- execution ordering
- immutable intent anchors
- tool authorization
- separated approval identities
- state and transition verification
- change provenance
- trace integrity
- fail-closed runtime verification

**Publication:** [Zenodo — AARC](https://doi.org/10.5281/zenodo.23107336)  
**DOI:** [`10.5281/zenodo.23107336`](https://doi.org/10.5281/zenodo.23107336)  
**ORCID:** [`0009-0002-1699-2043`](https://orcid.org/0009-0002-1699-2043)  
**Repository:** [Agentic Audit & Reliability Contract](https://github.com/SaridakisStamatisChristos/Agentic-Audit-Reliability-Contract-AARC-)

---

## 🧭 Current Focus

My current work is concentrated around the boundary between **model capability and execution correctness**.

A powerful model can still produce an unreliable autonomous system if the surrounding execution environment permits:

- invalid state transitions
- unauthorized tool calls
- duplicated side effects
- broken causal ordering
- unverifiable decisions
- silent policy violations
- unsafe retries
- corrupted recovery
- untraceable changes

I am particularly interested in architectures where autonomous systems operate through explicit execution contracts, verifiable traces, deterministic transitions, runtime policy enforcement, and recoverable state.

---

# Selected Engineering Work

## 🛡️ AegisRun / AEGIS

**Policy-enforced control plane for AI-agent tool execution.**

[View repository →](https://github.com/SaridakisStamatisChristos/AEGIS)

AegisRun places an enforcement layer between autonomous agents and the tools they invoke.

It combines:

- policy-as-code
- runtime execution budgets
- approval workflows
- tool authorization
- redaction
- tamper-evident evidence
- offline verification
- OIDC / RBAC
- tenant isolation
- observability
- backup and recovery
- Kubernetes-oriented deployment
- software-supply-chain evidence

The central design principle is that agent capability should not imply unrestricted execution authority.

---

## ✈️ CharterOS

**Deterministic transaction, procurement, operations, optimization, and evidence platform for B2B aviation charter.**

[View repository →](https://github.com/SaridakisStamatisChristos/CharterOS)

CharterOS models the charter lifecycle from mission creation and supplier sourcing through RFQs, quotes, tenders, award, booking, contracts, operations, disruption handling, financial reconciliation, and audit evidence.

The architecture emphasizes:

- PostgreSQL as canonical transactional authority
- deterministic state transitions
- bitemporal state
- immutable commercial lineage
- explicit authority boundaries
- transactional outbox patterns
- deterministic optimization
- auditable FX evidence
- graph projections
- no-hindsight historical semantics
- disaster recovery
- release provenance
- evidence reconstruction

The project explores how complex commercial workflows can remain explainable and auditable even under concurrency, retries, historical corrections, and automation.

---

## 🗄️ NeuralBase

**Experimental distributed SQL engine written in Rust.**

[View repository →](https://github.com/SaridakisStamatisChristos/Neuralbase)

NeuralBase explores the architecture of an AI-aware distributed database while retaining explicit correctness boundaries.

Implemented areas include:

- PostgreSQL wire protocol
- MVCC
- RocksDB persistence
- Raft-replicated mutations
- hybrid logical clocks
- vectorized execution
- SQL parsing and binding
- replicated identity state
- SCRAM authentication
- distributed membership management
- snapshots
- backup and restore
- exact committed-index recovery
- read-consistency modes
- compatibility testing
- reproducible performance characterization

The project treats distributed correctness, durability, recovery, and evidence as first-class system properties.

---

## 🌳 Merkle Evidence Vault

**Tamper-evident infrastructure for append-only evidence storage and offline verification.**

[View repository →](https://github.com/SaridakisStamatisChristos/merkle-evidence-vault)

The system combines:

- RFC 6962 Merkle trees
- Ed25519-signed checkpoints
- append-only evidence storage
- offline-verifiable evidence bundles
- authentication and authorization controls
- backup / restore drills
- adversarial fuzzing
- CI verification
- release governance
- reproducible evidence packaging

The broader goal is to make important system claims independently verifiable rather than dependent on trust in the originating service.

---

## ∑ Math Sentinel

**Stateful symbolic proof-agent research scaffold.**

[View repository →](https://github.com/SaridakisStamatisChristos/math-sentinel)

Math Sentinel explores reasoning systems where the authoritative object is an explicit **proof state**, rather than unrestricted generated text.

The architecture includes:

- explicit proof state
- typed reasoning actions
- deterministic mathematical tools
- prover / verifier separation
- verifier-guided beam search
- replay memory
- hard-case tracking
- persistent lemma memory
- procedural mathematical curricula

This project explores how generated reasoning can be constrained and evaluated through explicit machine-checkable state transitions.

---

## 🤖 StamCont

**Durable, provider-neutral coding-agent runtime.**

[View repository →](https://github.com/SaridakisStamatisChristos/StamCont)

StamCont focuses on the infrastructure required for long-running coding agents:

- durable sessions
- deterministic replay
- interruption-safe resume
- capability-scoped execution
- explicit execution profiles
- cross-platform sandboxing
- context compaction
- nested-agent authority
- cancellation propagation
- provider-neutral runtime events
- shared CLI / IDE semantics

The project originated from an imported Continue source baseline and retains the appropriate upstream attribution while developing a distinct durable agent-runtime architecture.

---

# Research & Engineering Interests

### Agentic Systems

- agent runtime assurance
- tool-using AI
- autonomous execution
- agent control planes
- execution traces
- approval systems
- state-transition verification
- multi-agent architectures
- runtime policy enforcement

### Distributed Systems

- consensus
- replication
- distributed databases
- transaction processing
- MVCC
- durability
- recovery
- event-driven systems
- distributed state machines

### Reliability & Verification

- invariant enforcement
- deterministic execution
- runtime verification
- auditability
- provenance
- reproducibility
- fail-closed architectures
- cryptographic evidence
- disaster recovery

### AI Reasoning Systems

- verifier-guided reasoning
- symbolic reasoning
- proof-state architectures
- tool-augmented models
- execution correctness
- model / runtime separation

### Optimization & Systems Engineering

- deterministic optimization
- high-performance computation
- data structures
- algorithm design
- workflow orchestration
- performance engineering

---

# Engineering Principles

Much of my work is built around a small number of recurring principles.

### Explicit state over implicit behavior

Important transitions should be represented explicitly and validated rather than inferred from loosely structured execution.

### Invariants over assumptions

Critical correctness properties should be encoded and continuously checked.

### Evidence over claims

Where possible, important assertions should be backed by tests, traces, benchmarks, cryptographic commitments, or reproducible artifacts.

### Determinism where it matters

Critical financial, transactional, authorization, and recovery paths should minimize hidden nondeterminism.

### Fail closed

When authority, state, evidence, or verification is incomplete, critical execution should not silently continue.

### Recovery is part of correctness

A system that behaves correctly during normal execution but cannot safely recover from interruption or partial failure is incomplete.

### Model intelligence ≠ execution reliability

An intelligent model can propose useful actions.

A reliable system must additionally determine:

1. whether the action is authorized,
2. whether the required invariants still hold,
3. whether execution is safe,
4. whether the resulting state can be verified,
5. and what should happen if execution partially fails.

---

# Technology

**Languages**

`Rust` · `Go` · `Python` · `TypeScript` · `SQL`

**Systems & Data**

`PostgreSQL` · `RocksDB` · `Raft` · `MVCC` · `REST` · `gRPC`

**Infrastructure**

`Docker` · `Kubernetes` · `GitHub Actions` · `Linux`

**Reliability & Security**

`OIDC` · `RBAC` · `SBOM` · `SLSA-style provenance` · `Fuzzing` · `Observability` · `Cryptographic verification`

**AI / Agent Systems**

`Tool-using agents` · `Agent runtimes` · `Execution verification` · `Policy enforcement` · `Symbolic reasoning`

---

# Research Identity

**Stamatis-Christos Saridakis**

Independent researcher and systems engineer.

**ORCID**  
[0009-0002-1699-2043](https://orcid.org/0009-0002-1699-2043)

**Zenodo**  
[AARC: A Machine-Verifiable Audit and Reliability Contract for Tool-Using AI Agents](https://doi.org/10.5281/zenodo.23107336)

**GitHub**  
[@SaridakisStamatisChristos](https://github.com/SaridakisStamatisChristos)

---

## Collaboration

I am interested in technically ambitious work involving:

- reliable autonomous agents
- agent infrastructure
- distributed systems
- database systems
- runtime assurance
- execution verification
- high-assurance software
- research engineering

Particularly interesting are projects where **correctness, reliability, and evidence matter as much as raw capability**.
