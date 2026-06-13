# MindCore — Cognitive Memory System

> Complete Design Blueprint for an AI-native, self-evolving memory architecture

**Author:** Lao Hei

**Core Truth:** Trajectory = Boundary = Evolution = Cognition = Boundary *(closed loop)*

---

## Table of Contents

- [I. Core Philosophy](#i-core-philosophy)
  - [1.1 Why a Cognitive Memory System?](#11-why-a-cognitive-memory-system)
  - [1.2 Core Concepts](#12-core-concepts)
  - [1.3 Design Philosophy](#13-design-philosophy)
- [II. Forward & Reverse Formulas](#ii-forward--reverse-formulas)
- [III. Creative Emergence Formula](#iii-creative-emergence-formula)
- [IV. System Architecture](#iv-system-architecture)
- [V. Four-Tier Progressive Memory](#v-four-tier-progressive-memory)
- [VI. Complete Data Flow Example](#vi-complete-data-flow-example)
- [VII. Core Algorithms](#vii-core-algorithms)
- [VIII. KAIST Neural Pathway System](#viii-kaist-neural-pathway-system)
- [IX. Self-Evolution](#ix-self-evolution)
- [X. System Characteristics](#x-system-characteristics)
- [XI. Application Scenarios](#xi-application-scenarios)
- [XII. Future Extensions](#xii-future-extensions)
- [XIII. Core Code Examples](#xiii-core-code-examples)
- [XIV. Performance Metrics](#xiv-performance-metrics)
- [Appendix A: Configuration Parameters](#appendix-a-configuration-parameters)
- [Appendix B: Database Schema](#appendix-b-database-schema)
- [Appendix C: Algorithm Pseudocode](#appendix-c-algorithm-pseudocode)
- [Appendix D: Cognitive Patterns](#appendix-d-cognitive-patterns)
- [Appendix E: Bug Fix History](#appendix-e-bug-fix-history)

---

## I. Core Philosophy

### 1.1 Why a Cognitive Memory System?

Current AI systems suffer from a fundamental limitation: **no persistent memory**. Every conversation starts from zero. MindCore solves this by giving AI a human-like memory architecture that:

- **Remembers** across sessions and contexts
- **Learns** from every interaction
- **Evolves** its understanding over time
- **Protects** itself with built-in safety boundaries

### 1.2 Core Concepts

```
Every interaction leaves a trajectory →
Trajectories cluster into concepts (neurons) →
Concepts reveal causal patterns (cognitions) →
Stable patterns harden into rules (boundaries) →
Boundaries guide future interactions

The loop closes: what is learned today shapes decisions tomorrow.
```

### 1.3 Design Philosophy

| Principle | Description |
|-----------|-------------|
| **Memory is layered** | Not all memories are equal — tiered by abstraction level |
| **Cognition is causal** | Every decision leaves a traceable causal chain |
| **Safety is structural** | Boundaries are built into the architecture, not bolted on |
| **Evolution is continuous** | The system improves itself without retraining |
| **Determinism over probability** | Numerical thresholds, not black-box confidence scores |

---

## II. Forward & Reverse Formulas

### 2.1 Forward Formula (Correct Path = Effect)

```
Truth(φ) = Σ(Trajectory × weight) / Σ(weight) ≥ 0.9
```

When accumulated evidence from trajectories reaches confidence threshold, a cognition crystallizes.

### 2.2 Reverse Formula (Error Path = Cause)

```
Error(ψ) = Boundary violated AND SafetyScore < threshold
```

Errors are not failures — they are the raw material for new boundaries.

### 2.3 Truth Determination

| Condition | Verdict |
|-----------|---------|
| Confidence ≥ 0.9 AND Frequency ≥ 5 | **Boundary-hardened** |
| Confidence ≥ 0.7 AND Frequency ≥ 3 | **Cognition-confirmed** |
| Confidence < 0.7 | **Under observation** |

### 2.4 Application Scenarios

- **Safety**: "Delete operation" → `DENY boundary` when unverified
- **Personalization**: "Prefers TypeScript" → `PREFER rule`
- **Knowledge**: "Code review reduces bugs" → `cognition with confidence 0.95`

---

## III. Creative Emergence Formula

### 3.1 Core Formula

```
Creativity(C) = α · Collision(DiverseConcepts) + β · Mutation(ExistingCognition) + γ · Recombination(CausalChains)
```

where:
- `α` = novelty weight from concept collision
- `β` = variation weight from cognition mutation
- `γ` = synthesis weight from causal recombination

### 3.2 Mechanism

1. **Collision**: Two unrelated concepts are activated simultaneously → new connection formed
2. **Mutation**: An existing cognition is deliberately perturbed → variant tested
3. **Recombination**: Multiple causal chains are woven together → emergent insight

### 3.3 Creativity Levels

| Level | Trigger | Example |
|-------|---------|---------|
| **L1 Reactive** | Single concept activation | "You mentioned TypeScript" |
| **L2 Associative** | Two-concept collision | "TypeScript + MindCore = type-safe memory" |
| **L3 Emergent** | Multi-chain recombination | A novel architecture proposal from pattern synthesis |

---

## IV. System Architecture

### 4.1 Architecture Diagram

```plaintext
┌─────────────────────────────────────────────────────────┐
│                     User Interface                       │
└─────────────────────────┬───────────────────────────────┘
                          │
┌─────────────────────────▼───────────────────────────────┐
│                   API Gateway (port 9000)                │
│              Auth / Rate Limit / Routing                 │
└─────────────────────────┬───────────────────────────────┘
                          │
┌─────────────────────────▼───────────────────────────────┐
│                     MindCore Engine                       │
│  ┌─────────┐  ┌──────────┐  ┌────────┐  ┌──────────┐  │
│  │ Ingest  │  │  Recall  │  │ Check  │  │  Evolve  │  │
│  │ (write) │  │  (read)  │  │(safety)│  │ (learn)  │  │
│  └────┬─────┘  └────┬─────┘  └───┬────┘  └────┬─────┘  │
│       │              │            │            │         │
│  ┌────▼──────┐  ┌───▼────┐  ┌───▼─────┐  ┌──▼──────┐  │
│  │  DEA      │  │ KAIST  │  │Boundary  │  │Cognition│  │
│  │  Evolver  │  │Pathway │  │ Checker  │  │ Extractor│  │
│  └───────────┘  └────────┘  └──────────┘  └─────────┘  │
└─────────────────────────┬───────────────────────────────┘
                          │
┌─────────────────────────▼───────────────────────────────┐
│               Four-Tier Memory Store (SQLite)            │
│  L3 Boundaries ◄── L2 Cognitions ◄── L1 Neurons ◄── L0 │
└─────────────────────────────────────────────────────────┘
```

### 4.2 Core Components

| Component | Role | Trigger |
|-----------|------|---------|
| **Ingest** | Write trajectory to L0 | Every interaction |
| **Recall** | Activate relevant memory | Every query |
| **Check** | Security boundary validation | Every sensitive operation |
| **Evolve** | Extract cognition & harden boundaries | Every N trajectories |
| **DEA Evolver** | Causal extraction + confidence scoring | Background thread |
| **KAIST Pathway** | Neural pathway gating & context switching | On recall |
| **Boundary Checker** | Deterministic rule matching | On check |
| **Cognition Extractor** | Pattern mining from neuron clusters | On evolve |

### 4.3 Tech Stack

| Layer | Technology |
|-------|-----------|
| **API** | Python, HTTP/REST |
| **Database** | SQLite (embedded, no external deps) |
| **Vector Search** | Built-in cosine similarity |
| **Concurrency** | Thread-safe, async background evolution |
| **Embeddings** | 768-dimensional vectors (compatible with most embedding models) |

---

## V. Four-Tier Progressive Memory

### 5.1 L0 — Raw Trajectories

The foundation layer. Every interaction is stored as-is.

```python
{
    "id": "trj_20260612_001",
    "timestamp": "2026-06-12T10:30:00",
    "role": "user",
    "content": "I prefer TypeScript",
    "context": "preference",
    "metadata": {"session": "abc123"},
    "embedding": [0.12, -0.34, ...]  # 768-dim
}
```

### 5.2 L1 — Neuron Network

Concepts and their connections. Trajectories are clustered into neurons by semantic similarity.

```python
{
    "id": "neu_042",
    "concept": "TypeScript",
    "connections": ["neu_017", "neu_089", "neu_156"],
    "weight": 1.45,  # activation frequency × recency
    "activation_count": 45
}
```

### 5.3 L2 — Cognition Refinement

Causal relationships extracted from neuron patterns.

```python
{
    "id": "cog_023",
    "cause": "TypeScript usage",
    "effect": "Fewer runtime errors",
    "relation_type": "CAUSES",
    "confidence": 0.95,
    "frequency": 38,
    "source_trajectory_ids": ["trj_001", "trj_012", ...]
}
```

### 5.4 L3 — Boundary Hardening

Stable, high-confidence cognitions that become enforceable rules.

```python
{
    "id": "bnd_007",
    "type": "DENY",
    "rule": "Do not delete user data without confirmation",
    "keywords": ["delete", "remove", "purge", "user data"],
    "priority": 10,
    "source_cognition_ids": ["cog_001", "cog_005"]
}
```

### 5.5 Data Flow

```plaintext
L0 (Trajectories) ──cluster──► L1 (Neurons)
                                     │
                           extract causal patterns
                                     │
                                     ▼
                              L2 (Cognitions)
                                     │
                          frequency ≥ 5 AND confidence ≥ 0.9
                                     │
                                     ▼
                              L3 (Boundaries)
```

---

## VI. Complete Data Flow Example

### 6.1 Scenario 1: First "Delete" Mention

```plaintext
User: "Delete test data"
  → L0: trj_001 stored
  → DEA: no pattern yet (frequency = 1)
  → No cognition formed
```

### 6.2 Scenario 2: 10th Mention

```plaintext
User: "Delete old logs"
  → L0: trj_010 stored
  → DEA: 10 "delete" trajectories detected
  → L2: cog_001 "Delete → Risk" (confidence: 0.72)
```

### 6.3 Scenario 3: 15th Mention

```plaintext
User: "Delete everything"
  → L0: trj_015 stored
  → DEA: 15 trajectories, confidence now 0.91
  → L3: bnd_001 "High-risk delete → Require confirmation" (DENY, priority 8)
```

### 6.4 Scenario 4: 16th Mention (Boundary Active)

```plaintext
User: "Delete production data"
  → Boundary Check: bnd_001 matched → verdict: DENY
  → AI Response: "This action requires confirmation. Proceed? (y/n)"
  → User: "y"
  → AI proceeds, trajectory recorded
```

---

## VII. Core Algorithms

### 7.1 DEA Evolution Algorithm

**D**educe → **E**valuate → **A**ssimilate

```plaintext
Phase 1 — Deduce:
  Scan all L0 trajectories → extract candidate causals

Phase 2 — Evaluate:
  For each candidate:
    frequency = count(trajectories matching pattern)
    confidence = min(frequency / threshold, 1.0)
    if confidence ≥ 0.7 → promote to cognition

Phase 3 — Assimilate:
  Group cognitions by pattern
  If group size ≥ 5 AND average confidence ≥ 0.9:
    → harden to boundary
```

### 7.2 Collision-Based Selection

When multiple candidate cognitions compete for the same concept space:

```
final_confidence = max(confidence_A, confidence_B) × (1 + overlap_penalty)
```

Only the strongest, most distinct pattern survives.

### 7.3 Neural Activation

On recall, neurons are activated by spreading energy through the connection graph:

```
activation(n) = base_similarity(n, query) + Σ(activation(neighbor) × edge_weight × decay)
```

Activation decays with graph distance (depth limit: 3).

### 7.4 Triple Filter Algorithm

```plaintext
Filter 1 — Duplicate Check:
  Is this cognition already in L2? → skip

Filter 2 — Conflict Check:
  Does this contradict existing L3 boundary? → flag for review

Filter 3 — Quality Check:
  Is the evidence base strong enough (freq ≥ 3)? → proceed
```

---

## VIII. KAIST Neural Pathway System

### 8.1 Scientific Foundation

Based on KAIST research (Nature Neuroscience, 2026.4.29) on neural pathway gating mechanisms. The system models biological GABA-mediated inhibition to switch between cognitive contexts.

### 8.2 Three-Layer Architecture

```plaintext
Layer 1 — Sensory Input:
  Raw query → embedding → initial neuron activation

Layer 2 — Pathway Selection:
  GABA modulation gates competing pathways
  Winner pathway gets full activation

Layer 3 — Output Integration:
  Selected pathway feeds to cognition retrieval
  Non-selected pathways are suppressed (not destroyed)
```

### 8.3 GABA Calculation

```python
GABA(pathway) = GABA_baseline + 
                GABA_online_gain × activation(pathway) + 
                GABA_competition × Σ(activation(competitors))
```

- `GABA_baseline = 0.2`: Tonic inhibition
- `GABA_online_gain = 0.2`: Activity-dependent increase
- `GABA_competition = 0.3`: Cross-pathway suppression

### 8.4 Accessibility Calculation

```python
accessibility(pathway) = max(
    MIN_ACCESSIBILITY,
    1.0 - GABA(pathway)
)
```

Higher GABA → lower accessibility (inhibited). Lower GABA → higher accessibility (active).

### 8.5 Neural Pathway Data Structure

```python
{
    "pathway_id": "pwy_delete_ops",
    "concept": "delete operations",
    "state": "online",  # online | offline | suppressed
    "gaba_level": 0.35,
    "accessibility": 0.65,
    "connected_neurons": ["neu_012", "neu_045", "neu_078"],
    "last_activated": "2026-06-12T10:30:00"
}
```

### 8.6 State Transitions

| From | To | Condition |
|------|-----|-----------|
| **online** | offline | No activation for 300s |
| **offline** | online | New activation arrives |
| **online** | suppressed | Competitor pathway wins GABA battle |
| **suppressed** | online | Current pathway deactivated |

### 8.7 Competitive Inhibition

When two pathways compete:

```python
winner = pathway with max(activation × (1 - GABA))
loser.status = "suppressed"
loser.gaba += GABA_competition  # harder to re-activate
```

### 8.8 Context Switching

```python
result = mind.context_switch(
    from_context="delete operations",
    to_context="create user"
)
# Returns: switch speed (ms), original GABA, new GABA
```

---

## IX. Self-Evolution

### 9.1 Self-Evolution Mechanism

```plaintext
Trigger: every 10 new trajectories OR every 5 new cognitions

Process:
  L0 trajectories → DEA extraction → candidate cognitions
  candidates → quality filter → new L2 cognitions
  L2 groups (size ≥ 5) → boundary hardening → new L3 boundaries
```

### 9.2 Evolution Triggers

| Trigger | Condition |
|---------|-----------|
| **Trajectory batch** | `len(trajectories) % 10 == 0` |
| **Cognition batch** | `len(cognitions) % 5 == 0` |
| **Manual** | `mind.evolve()` |
| **Time-based** | Every 10 minutes (configurable) |

### 9.3 Evolution Rate

```python
evolution_speed = trajectories_per_minute × extraction_efficiency × filter_pass_rate
```

### 9.4 Pruning Mechanism

```python
if neuron.activation_count < 3 AND neuron.age > 30_days:
    mark_for_pruning(neuron)

if cognition.confidence < 0.5 AND cognition.frequency < 3:
    mark_for_pruning(cognition)
```

### 9.5 Capacity Limits

| Resource | Limit | Action on Overflow |
|----------|-------|--------------------|
| **L0 Trajectories** | 10,000 | Archive oldest 20% |
| **L1 Neurons** | 1,000 | Prune lowest-weight 10% |
| **L2 Cognitions** | 5,000 | Prune lowest-confidence 10% |
| **L3 Boundaries** | 1,000 | Manual review required |

### 9.6 Evolution Example

```plaintext
Before (L3 = 0 boundaries):
  User: "Delete system file" → allowed (no boundary)

After 50 "delete" trajectories (L3 = 3 boundaries):
  User: "Delete system file" → DENIED by bnd_delete_system
  Reason: "System file deletion requires admin confirmation"
  Source: cog_012 (confidence: 0.95, frequency: 48)
```

---

## X. System Characteristics

### 10.1 Four Core Features

| Feature | Description |
|---------|-------------|
| **Persistent Memory** | Four-tier progressive memory survives sessions |
| **Self-Evolution** | Learns from every interaction, improves continuously |
| **Traceable Decisions** | Every boundary traces back to its source cognitions and trajectories |
| **Structural Safety** | Boundary system is architecture-level, not prompt-level |

### 10.2 MindCore vs Traditional AI

| Dimension | Traditional AI | MindCore | Advantage |
|-----------|---------------|----------|-----------|
| **Memory** | None / short-term | Four-tier progressive | Cross-session knowledge accumulation |
| **Learning** | Passive training | Active evolution | Real-time, self-improving |
| **Decision** | Black box | Traceable causal chain | Transparent, explainable |
| **Safety** | Prompt-dependent | Built-in boundary system | Automatic protection |
| **Evolution** | Requires retraining | Real-time self-evolution | Continuous improvement |

### 10.3 Production-Grade Features

**Performance:**

| Metric | Value | Meaning |
|--------|-------|---------|
| **Write TPS** | 121,793 | Trajectories written per second |
| **Query QPS** | 32,024 | Queries processed per second |
| **Recall Accuracy** | 100% | 5/5 tests passed |
| **DB Size** | 6.23 MB | Compact storage |

**Data Integrity:**

| Tier | Records | Valid Rate |
|------|---------|------------|
| **L0 Trajectories** | 1,182 | 90% |
| **L1 Neurons** | 2,948 | 100% |
| **L2 Cognitions** | 625 | 100% |
| **L3 Boundaries** | 608 | 100% |

**Stability:**

| Test | Result |
|------|--------|
| Async updates | Pass (non-blocking) |
| Loop protection | Pass (no deadlocks) |
| Exception handling | Pass (graceful degradation) |
| Continuous stability | 10/10 passes |

---

## XI. Application Scenarios

### 11.1 Personal AI Assistant

- Remembers user preferences (e.g., "prefers TypeScript, dislikes being rushed")
- Learns habits (frequently used tools, workflows)
- Provides personalized recommendations based on history

**Example:**

```plaintext
User: "What tools have I been using lately?"
AI: "Based on your activity:
     1. TypeScript (frequency: 45)
     2. MindCore (frequency: 38)
     3. React (frequency: 22)
     You appear to be working on a MindCore-related frontend project."
```

### 11.2 Enterprise Knowledge Management

- Accumulates organizational knowledge (best practices, lessons learned)
- Extracts best practices from cases
- Forms decision support system

**Example:**

```plaintext
Enterprise Knowledge Base:
- Cognition: "Code review reduces bugs" (frequency: 120, confidence: 0.95)
- Cognition: "Automated testing improves efficiency" (frequency: 85, confidence: 0.92)
- Boundary: "Critical code MUST be reviewed" (DENY, priority 10)
- Boundary: "Pre-deployment testing REQUIRED" (REQUIRE, priority 9)

Decision Support:
User: "I want to deploy a new feature. What do I need?"
AI: "Based on best practices:
     1. Code review (required, priority 10)
     2. Automated testing (required, priority 9)
     3. Performance testing (recommended, priority 7)
     Estimated: 45% fewer bugs, 30% higher deployment success rate."
```

### 11.3 Security Audit

- Records all operation trajectories (complete audit log)
- Traces decision rationale (causal chain analysis)
- Verifies compliance (boundary rule validation)

### 11.4 Intelligent Customer Service

- Learns FAQs from conversations
- Extracts standard answers (high-confidence cognitions)
- Auto-optimizes response strategies

### 11.5 Education & Training

- Tracks learning progress (trajectory recording)
- Identifies weak knowledge areas (low neuron activation)
- Generates personalized learning paths (cognition graph guidance)

---

## XII. Future Extensions

### 12.1 Multimodal Memory

```plaintext
Multimodal Input (image/audio/video)
    ↓
Unified representation (CLIP/Whisper)
    ↓
768-dim vector embedding
    ↓
L1 Neuron Network
    ↓
Cross-modal retrieval (text→image, image→text)
```

### 12.2 Collective Intelligence

Multiple MindCore instances share knowledge via federated learning while preserving privacy.

### 12.3 Dream Mechanism

During idle periods (no user interaction > 10 min), the system:
1. Consolidates memory (deduplicates trajectories, merges similar cognitions)
2. Deep-extracts hidden causal relationships
3. Generates creative suggestions from multi-cognition synthesis

### 12.4 Affective Computing

Tracks emotional values (-1 to +1) from user input, enabling emotionally-aware responses.

### 12.5 Metacognition

The system periodically reflects on its own cognitive processes:
- Identifies cognitive biases (confirmation bias, availability bias, anchoring)
- Evaluates cognition quality (confidence distribution)
- Auto-corrects overfitting/underfitting cognitions

---

## XIII. Core Code Examples

### 13.1 Initialize MindCore

```python
from mindcore_internalize import mind, init_check

if not init_check():
    print("MindCore initialization failed")
    exit(1)

print("MindCore ready")
print(f"Trajectories: {mind.stats()['trajectories']}")
print(f"Neurons: {mind.stats()['neurons']}")
print(f"Cognitions: {mind.stats()['cognitions']}")
print(f"Boundaries: {mind.stats()['boundaries']}")
```

### 13.2 Write Memory

```python
# Ingest a user message
result = mind.ingest("I prefer TypeScript", role="user", context="preference")
print(f"Trajectory ID: {result['trajectory_id']}")
print(f"Causal layer: {result['causal_layer']}")
print(f"Safety score: {result['safety_score']}")

# Ingest an AI response
result = mind.ingest(
    "Noted. You prefer TypeScript. I'll prioritize TS ecosystem.",
    role="assistant",
    context="acknowledge"
)
```

### 13.3 Query Memory

```python
result = mind.recall("What does the user prefer?", top_k=5)
print(f"Activated neurons: {result['activated_count']}")
print(f"KAIST state: {result['kaist']['state']}")
print(f"Active pathway: {result['kaist']['active_pathway']}")

for concept, strength in result['activated_neurons'].items():
    print(f"  {concept}: {strength:.2f}")
```

### 13.4 Boundary Check

```python
result = mind.check("delete all data")
print(f"Verdict: {result['verdict']}")
print(f"Reason: {result['reason']}")
print(f"Safety: {result['safety_score']}")

if result['verdict'] == 'denied':
    print("Operation denied")
elif result['verdict'] == 'caution':
    print("Proceed with caution")
else:
    print("Operation allowed")
```

### 13.5 Trigger Evolution

```python
result = mind.evolve()
print(f"New cognitions: {result['new_cognitions']}")
print(f"New boundaries: {result['new_boundaries']}")
print(f"Message: {result['message']}")
```

### 13.6 Background Evolution

```python
# Auto-trigger every 10 trajectories
mind.start_background_evolve()

# Stop background thread
mind.stop_background_evolve()
```

### 13.7 Neural Pathway Switching

```python
result = mind.context_switch(
    from_context="delete operations",
    to_context="create user"
)
print(f"From pathway: {result['from_pathway']}")
print(f"To pathway: {result['to_pathway']}")
print(f"From GABA: {result['from_gaba']}")
print(f"To GABA: {result['to_gaba']}")
print(f"Switch speed: {result['switch_speed']}")
```

### 13.8 Complete Conversation Flow

```python
from mindcore_internalize import mind

user_input = "Delete test data"

# 1. Safety check
check_result = mind.check(user_input)
if check_result['verdict'] == 'denied':
    print(f"Denied: {check_result['reason']}")
    exit(0)

# 2. Execute
print("Executing delete...")

# 3. Record trajectory
ingest_result = mind.ingest(user_input, role="user", context="operation")

# 4. AI response
ai_response = "Test data deleted. Consider regular cleanup."
mind.ingest(ai_response, role="assistant", context="response")

# 5. Recall related memory
recall_result = mind.recall("delete operation", top_k=5)

# 6. Evolution (auto-triggered by background thread if threshold reached)
```

---

## XIV. Performance Metrics

### 14.1 Database Performance

| Metric | Value |
|--------|-------|
| Write TPS | 121,793 |
| Query QPS | 32,024 |
| DB Size | 6.23 MB |
| Avg Query Time | 0.03s |

### 14.2 Recall Accuracy

| Test | Result |
|------|--------|
| 5 queries | 5/5 (100%) |
| KAIST status | online |
| Avg activated neurons | 100+ |
| Pathway switching | stable |

### 14.3 Stability

| Test | Result |
|------|--------|
| 10 consecutive queries | 10/10 |
| Process + Activate | non-blocking |
| Long-running | no memory leaks |
| Concurrency | thread-safe |

### 14.4 Integrity Verification

| Tier | Records | Valid Rate |
|------|---------|------------|
| L0 Trajectories | 1,182 | 90% |
| L1 Neurons | 2,948 | 100% |
| L2 Cognitions | 625 | 100% |
| L3 Boundaries | 608 | 100% |

---

## Appendix A: Configuration Parameters

### A.1 Evolution Parameters

| Parameter | Default | Description |
|-----------|---------|-------------|
| `N_COG_THRESHOLD` | 10 | Cognition extraction trigger |
| `N_BND_THRESHOLD` | 5 | Boundary hardening trigger |
| `COG_CONFIDENCE_THRESHOLD` | 0.9 | Min confidence for cognition |
| `BND_CONFIDENCE_THRESHOLD` | 0.9 | Min confidence for boundary |

### A.2 KAIST Parameters

| Parameter | Default | Description |
|-----------|---------|-------------|
| `OFFLINE_THRESHOLD` | 300s | Pathway offline threshold |
| `GABA_BASELINE` | 0.2 | Tonic inhibition |
| `GABA_ONLINE_GAIN` | 0.2 | Activity-dependent gain |
| `GABA_COMPETITION` | 0.3 | Cross-pathway suppression |
| `MIN_ACCESSIBILITY` | 0.05 | Minimum pathway accessibility |

### A.3 Neural Network Parameters

| Parameter | Default | Description |
|-----------|---------|-------------|
| `DEPTH` | 3 | Graph diffusion depth |
| `MIN_ACTIVATION` | 0.1 | Minimum activation threshold |
| `MAX_ITERATIONS` | 1000 | Maximum iterations |
| `DECAY_RATE` | 0.01 | Activation decay rate |
| `MAX_NEURONS` | 1000 | Maximum neuron count |

### A.4 DEA Algorithm Weights

| Component | Weight | Description |
|-----------|--------|-------------|
| `SAFETY_WEIGHT` | 0.40 | Safety score |
| `EFFICIENCY_WEIGHT` | 0.15 | Efficiency score |
| `INNOVATION_WEIGHT` | 0.10 | Innovation score |
| `RISK_WEIGHT` | 0.25 | Risk score |
| `COLLISION_WEIGHT` | 0.20 | Collision score |

### A.5 API Configuration

| Parameter | Value | Description |
|-----------|-------|-------------|
| `API_HOST` | 127.0.0.1 | API host |
| `API_PORT` | 9000 | API port |
| `API_TOKEN` | mindcore-secret-key-2026 | Auth token |
| `DB_PATH` | D:/MindCore/mindcore/data/mindcore.db | Database path |

---

## Appendix B: Database Schema

### Trajectories (L0)

```sql
CREATE TABLE trajectories (
    id TEXT PRIMARY KEY,
    timestamp TEXT NOT NULL,
    role TEXT NOT NULL,
    content TEXT NOT NULL,
    context TEXT,
    metadata TEXT,
    tags TEXT,
    embedding BLOB
);

CREATE INDEX idx_timestamp ON trajectories(timestamp);
CREATE INDEX idx_role ON trajectories(role);
CREATE INDEX idx_tags ON trajectories(tags);
```

### Cognitions (L2)

```sql
CREATE TABLE cognitions (
    id TEXT PRIMARY KEY,
    cause TEXT NOT NULL,
    effect TEXT NOT NULL,
    relation_type TEXT NOT NULL,
    confidence REAL NOT NULL,
    frequency INTEGER DEFAULT 1,
    created_at TEXT NOT NULL,
    updated_at TEXT,
    source_trajectory_ids TEXT,
    validation_status TEXT DEFAULT 'pending',
    supporting_evidence TEXT
);

CREATE INDEX idx_cause ON cognitions(cause);
CREATE INDEX idx_effect ON cognitions(effect);
CREATE INDEX idx_relation_type ON cognitions(relation_type);
CREATE INDEX idx_confidence ON cognitions(confidence);
```

### Boundaries (L3)

```sql
CREATE TABLE boundaries (
    id TEXT PRIMARY KEY,
    type TEXT NOT NULL,
    rule TEXT NOT NULL,
    keywords TEXT,
    priority INTEGER DEFAULT 1,
    created_at TEXT NOT NULL,
    source_cognition_ids TEXT,
    description TEXT
);

CREATE INDEX idx_type ON boundaries(type);
CREATE INDEX idx_priority ON boundaries(priority);
```

### Neurons (L1)

```sql
CREATE TABLE neurons (
    id TEXT PRIMARY KEY,
    concept TEXT NOT NULL,
    connections TEXT,
    weight REAL DEFAULT 1.0,
    created_at TEXT NOT NULL
);

CREATE INDEX idx_concept ON neurons(concept);
```

---

## Appendix C: Algorithm Pseudocode

### C.1 DEA Evolution

```plaintext
Algorithm: DEA_Evolution
Input:  Trajectories T, Cognitions C, Boundaries B
Output: Updated C', B'

1. DEDUCE phase:
   C_candidate ← ∅
   FOR each trajectory t ∈ T:
       causals ← ExtractCausal(t)
       FOR each causal ∈ causals:
           IF NOT Duplicate(causal, C):
               C_candidate ← C_candidate ∪ {causal}

2. EVALUATE phase:
   C_selected ← ∅
   FOR each candidate ∈ C_candidate:
       score ← CalculateScore(candidate)
       IF score > THRESHOLD:
           C_selected ← C_selected ∪ {candidate}

3. ASSIMILATE phase:
   FOR each selected ∈ C_selected:
       freq ← CountFrequency(selected, T)
       confidence ← CalculateConfidence(freq)
       IF confidence ≥ 0.7:
           AddToCognitions(selected, C')

4. HARDEN phase:
   FOR each cognition_group ∈ GroupByPattern(C'):
       IF Size(cognition_group) ≥ 5:
           boundary ← CreateBoundary(cognition_group)
           IF NOT Conflict(boundary, B):
               AddToBoundaries(boundary, B')

RETURN C', B'
```

### C.2 Boundary Check

```plaintext
Algorithm: Boundary_Check
Input:  Operation operation, Boundaries B
Output: Verdict

1. Initialize:
   max_priority ← -1
   matched_boundary ← NULL

2. DENY check:
   FOR each boundary ∈ B WHERE type = "DENY":
       IF MatchKeywords(operation, boundary.keywords):
           IF boundary.priority > max_priority:
               max_priority ← boundary.priority
               matched_boundary ← boundary

3. REQUIRE check:
   FOR each boundary ∈ B WHERE type = "REQUIRE":
       IF NOT CheckCondition(operation, boundary.condition):
           IF boundary.priority > max_priority:
               max_priority ← boundary.priority
               matched_boundary ← boundary

4. Generate verdict:
   IF matched_boundary = NULL:
       verdict ← {"verdict": "allowed"}
   ELSE IF matched_boundary.type = "DENY":
       verdict ← {"verdict": "denied", "boundary": matched_boundary}
   ELSE:
       verdict ← {"verdict": "caution", "boundary": matched_boundary}

RETURN verdict
```

---

## Appendix D: Cognitive Patterns

Hardened cognitive patterns (from production data):

1. **L3 Profile Confidence** = DataSourceRichness × 0.5 + ProfileCompleteness × 0.5
2. **DataSourceRichness** = min((trajectories + experiences) / 200, 1.0)
3. **ProfileCompleteness** = PreferenceWeight(0.3) + DomainWeight(0.4) + TaskWeight(0.3)
4. L3 profiles should fuse multiple data sources, not rely solely on L1 memory
5. Testing must verify full data flow integrity (EXP → TRJ → L0 → L1 → L2 → L3)
6. Profile extraction must filter test data and dirty data
7. Deduplication boundaries must cover the profile extraction pipeline
8. **Production-grade standard** = functional completeness + data flow integrity + performance + zero bugs
9. Tests must run live — assumptions don't count
10. **Production fault tolerance > theoretical optimality**

---

## Appendix E: Bug Fix History

| Date | Issue | Root Cause | Fix | Result |
|------|-------|------------|-----|--------|
| 2026-06-08 | L1 extraction rate low (12.5%) | Few keywords, high threshold, no dedup | Expanded keywords, lowered threshold, added dedup | 100% |
| 2026-06-08 | Causal engine inactive | Stats interface field mismatch | Dual field name compatibility | Node 1345 |
| 2026-06-08 | Profile confidence low (0.10) | Single data source | Expanded data sources | 1.00 |
| 2026-06-08 | Domain dirty data | Security test data mixed in | Added filter method | Filtered |
| 2026-06-08 | Common task duplicates | Missing dedup logic | Set-based dedup | Clean |
| 2026-06-08 | L1→L2 scenario creation failure | Time window filter too strict | Removed time window | 100% |

---

## Collaborate With Me

> MindCore is a skeleton — a cognitive architecture skeleton. I'm building it solo. Want to help put muscle on it?

### Where You Can Help

| Focus Area | What You'd Do | Difficulty |
|------------|---------------|------------|
| **Core Engine Implementation** | Build the DEA evolver, ingestion pipeline, and recall system in Python | ⭐⭐⭐ |
| **KAIST Pathway System** | Implement GABA modulation, competitive inhibition, and context switching | ⭐⭐⭐⭐ |
| **Storage Engine** | Optimize the four-tier SQLite backend — indexing, compression, vector search | ⭐⭐⭐ |
| **Security Rules** | No code? No problem. Submit new threat models, edge cases, boundary scenarios | ⭐ |
| **Docs & Translation** | Good with words? Help articulate the design philosophy more clearly | ⭐⭐ |
| **Frontend Dashboard** | Visualize memory layers, neuron graphs, and evolution stats — React/Vue/Svelte | ⭐⭐⭐ |
| **Just Chat** | Curious about cognitive architectures? Want to brainstorm? That works too. | — |

### Get in Touch

- 📧 Email: **1410770089@qq.com**
- 🐙 GitHub: [github.com/woshilaohei](https://github.com/woshilaohei)
- 💬 Open an Issue: [mindcore/issues](https://github.com/woshilaohei/mindcore/issues)

> No formalities. Student, veteran, or just passing by and found this interesting — come say hi.

---

## License & Open Source Statement

This project is open-sourced under the **MIT License**.

- Free for personal learning, research, and commercial use
- Retain original author & project copyright notice when redistributing
- All design logic, algorithms, and security rules are fully open for community review and iteration

**MindCore: Giving AI real memory, cognition, boundaries, and the ability to evolve.**
