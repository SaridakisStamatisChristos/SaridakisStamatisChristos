# Stamatis-Christos Saridakis

### Systems Engineer · Independent Researcher

[ORCID](https://orcid.org/0009-0002-1699-2043) · [Execution Assurance Preprint](https://doi.org/10.5281/zenodo.23119087) · [AARC Preprint](https://doi.org/10.5281/zenodo.23107336) · [GitHub](https://github.com/SaridakisStamatisChristos)

I build **reliability-focused software for agentic AI, distributed systems, databases, transactional platforms, and verifiable infrastructure**.

My work is organized around one recurring question:

> **How do we make increasingly autonomous software remain correct, auditable, recoverable, and controllable across multi-step execution?**

I explore that problem through runtime assurance, explicit state transitions, invariant enforcement, deterministic execution, cryptographic evidence, recovery semantics, and systems that separate **model capability** from **execution authority**.

---

## 📄 Published Research

### Agentic Execution Assurance: Observation-Bounded Certification, Runtime Enforcement, and Tamper-Evident Evidence

**Zenodo preprint v2.1** · DOI [10.5281/zenodo.23119087](https://doi.org/10.5281/zenodo.23119087)

This paper develops a bounded execution-assurance framework for tool-using AI agents by coupling **observation-bounded certification, typed pre-effect enforcement, claim-dependent evidence semantics, and a source-audited reference implementation**.

It formalizes when execution properties can be certified from an observation boundary, scopes runtime safety guarantees to mediated committed effects, distinguishes cryptographic integrity from semantic truth, and evaluates the resulting assurance boundaries against the pinned AegisRun / AEGIS implementation.

- **Preprint:** [10.5281/zenodo.23119087](https://doi.org/10.5281/zenodo.23119087)
- **Reproducibility artifact:** [10.5281/zenodo.23118665](https://doi.org/10.5281/zenodo.23118665)
- **Reference implementation:** [AegisRun / AEGIS](https://github.com/SaridakisStamatisChristos/AEGIS)
- **ORCID:** [0009-0002-1699-2043](https://orcid.org/0009-0002-1699-2043)

### AARC — A Machine-Verifiable Audit and Reliability Contract for Tool-Using AI Agents

**Zenodo preprint v1.1.1** · DOI [10.5281/zenodo.23107336](https://doi.org/10.5281/zenodo.23107336)

AARC specifies a machine-verifiable execution contract for tool-using AI agents using **externally observable runtime evidence rather than hidden chain-of-thought**.

It focuses on execution ordering, immutable intent anchors, tool authorization, separated approval identities, state verification, trace integrity, and change provenance.

- **Zenodo:** [AARC preprint](https://doi.org/10.5281/zenodo.23107336)
- **ORCID:** [0009-0002-1699-2043](https://orcid.org/0009-0002-1699-2043)
- **Repository:** [Agentic Audit & Reliability Contract](https://github.com/SaridakisStamatisChristos/Agentic-Audit-Reliability-Contract-AARC-)

---

## 🧭 Current Focus

A capable model does not automatically produce a reliable autonomous system.

The surrounding runtime must still determine:

1. whether an action is authorized,
2. whether required invariants still hold,
3. whether execution is safe,
4. whether the resulting state can be verified,
5. and how the system should recover if execution partially fails.

That boundary between **intelligence and execution correctness** is the central theme connecting much of my current engineering and research.

---

## 🚀 Selected Engineering Work

### 🛡️ [AegisRun / AEGIS](https://github.com/SaridakisStamatisChristos/AEGIS)

**Policy-enforced control plane for AI-agent tool execution.**

AegisRun places an enforcement layer between autonomous agents and the tools they invoke, combining policy-as-code, approvals, execution budgets, redaction, tamper-evident evidence, offline verification, OIDC/RBAC, observability, and operational controls.

**Core idea:** agent capability should never imply unrestricted execution authority.

---

### ✈️ [CharterOS](https://github.com/SaridakisStamatisChristos/CharterOS)

**Deterministic transaction, procurement, operations, optimization, and evidence platform for B2B aviation charter.**

CharterOS models the charter lifecycle across sourcing, RFQs, quotes, tenders, award, booking, contracts, operations, disruption handling, reconciliation, and audit evidence.

The architecture emphasizes PostgreSQL as canonical authority, bitemporal state, immutable commercial lineage, deterministic optimization, transactional outboxes, auditable FX, no-hindsight semantics, explicit authority boundaries, recovery, and release provenance.

---

### 🗄️ [NeuralBase](https://github.com/SaridakisStamatisChristos/Neuralbase)

**Experimental distributed SQL engine written in Rust.**

NeuralBase combines PostgreSQL wire compatibility, MVCC, RocksDB persistence, Raft-replicated mutations, hybrid logical clocks, vectorized execution, replicated identity state, snapshots, backup/restore, recovery semantics, explicit read-consistency modes, and reproducible performance characterization.

**Core idea:** distributed correctness, durability, and recovery are first-class system properties rather than operational afterthoughts.

---

### 🌳 [Merkle Evidence Vault](https://github.com/SaridakisStamatisChristos/merkle-evidence-vault)

**Tamper-evident infrastructure for append-only evidence storage and offline verification.**

The system uses RFC 6962 Merkle trees, Ed25519-signed checkpoints, append-only storage, offline-verifiable evidence bundles, authentication controls, recovery drills, fuzzing, CI verification, and release-governance evidence.

**Core idea:** important system claims should be independently verifiable rather than dependent on trust in the originating service.

---

### ∑ [Math Sentinel](https://github.com/SaridakisStamatisChristos/math-sentinel)

**Stateful symbolic proof-agent research scaffold.**

Math Sentinel explores reasoning systems where the authoritative object is an explicit **proof state**, not unrestricted generated text. It combines typed actions, deterministic mathematical tools, prover/verifier separation, verifier-guided search, replay, hard-case tracking, and persistent lemma memory.

---

### 🤖 [StamCont](https://github.com/SaridakisStamatisChristos/StamCont)

**Durable, provider-neutral coding-agent runtime.**

StamCont focuses on long-running agent execution: durable sessions, deterministic replay, interruption-safe resume, capability-scoped execution, cross-platform sandboxing, context compaction, nested-agent authority, cancellation propagation, and shared CLI/IDE runtime semantics.

StamCont originated from an imported Continue source baseline and retains the appropriate upstream attribution while developing a distinct durable agent-runtime architecture.

---

## 🔬 Research & Engineering Interests

**Agentic systems**  
Runtime assurance · tool-using AI · autonomous execution · agent control planes · execution traces · approval systems · state-transition verification · runtime policy enforcement

**Distributed systems**  
Consensus · replication · distributed databases · transaction processing · MVCC · durability · recovery · event-driven systems · distributed state machines

**Reliability & verification**  
Invariant enforcement · deterministic execution · runtime verification · auditability · provenance · reproducibility · fail-closed architecture · cryptographic evidence · disaster recovery

**AI reasoning systems**  
Verifier-guided reasoning · symbolic reasoning · proof-state architectures · tool-augmented models · model/runtime separation

**Optimization & systems engineering**  
Deterministic optimization · high-performance computation · data structures · algorithm design · workflow orchestration · performance engineering

---

## 🧱 Engineering Principles

- **Explicit state over implicit behavior** — important transitions should be represented and validated directly.
- **Invariants over assumptions** — critical correctness properties should be encoded and continuously checked.
- **Evidence over claims** — tests, traces, benchmarks, cryptographic commitments, and reproducible artifacts should support important assertions.
- **Determinism where it matters** — critical transactional, financial, authorization, and recovery paths should minimize hidden nondeterminism.
- **Fail closed** — incomplete authority, state, or verification should not silently become permission to continue.
- **Recovery is part of correctness** — safe resume, rollback, replay, and partial-failure handling belong in the core design.
- **Model intelligence ≠ execution reliability** — intelligent proposals still require controlled, verifiable execution.

---

## 🛠️ Technology

**Languages:** Rust · Go · Python · TypeScript · SQL

**Systems & Data:** PostgreSQL · RocksDB · Raft · MVCC · REST · gRPC

**Infrastructure:** Docker · Kubernetes · GitHub Actions · Linux

**Reliability & Security:** OIDC · RBAC · SBOM · SLSA-style provenance · fuzzing · observability · cryptographic verification

**AI / Agent Systems:** tool-using agents · agent runtimes · execution verification · policy enforcement · symbolic reasoning

---

## 🧑‍🔬 Research Identity

**Stamatis-Christos Saridakis**  
Independent Researcher & Systems Engineer

- **ORCID:** [0009-0002-1699-2043](https://orcid.org/0009-0002-1699-2043)
- **Zenodo:** [Agentic Execution Assurance](https://doi.org/10.5281/zenodo.23119087)
- **Artifact:** [Reproducibility Artifact](https://doi.org/10.5281/zenodo.23118665)
- **Zenodo:** [AARC — Machine-Verifiable Audit and Reliability Contract](https://doi.org/10.5281/zenodo.23107336)
- **GitHub:** [@SaridakisStamatisChristos](https://github.com/SaridakisStamatisChristos)

---

## 🤝 Collaboration

I am interested in technically ambitious work involving **reliable autonomous agents, agent infrastructure, distributed systems, database systems, runtime assurance, execution verification, and high-assurance software**.

The projects I find most interesting are those where **correctness, reliability, and evidence matter as much as raw capability**.
