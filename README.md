# 🚀 Telepathic AI: Recursive Multi-Agent Systems (RecursiveMAS)

Telepathic AI introduces a new paradigm for multi-agent systems by enabling **direct latent-space communication** between AI agents. Instead of relying on slow and lossy natural language exchanges, agents share high-dimensional internal representations — allowing for faster, richer, and more coherent collaboration.

---

## 🧠 Core Concept: "Telepathic" Communication

### ❌ Traditional Approach (Text-Based Communication)
- Agents communicate via natural language  
- Introduces a **discrete bottleneck**  
- Loss of nuance and reasoning fidelity  
- Slower interaction cycles  

### ✅ Telepathic AI Approach
- Agents exchange **latent states (hidden vectors)** directly  
- Preserves full reasoning context  
- Enables **continuous, differentiable communication**  
- Transforms a swarm into a unified neural system  

> Instead of sending messages, agents share their *thought-space*.

---

## 🏗️ Repository Architecture
- modeling.py # RecursiveLink + latent communication core
-  run.py # Main execution engine for recursive swarms
- system_loader.py # Loads models and initializes links
- hf_resolver.py # Resolves HuggingFace weights and adapters
- inference_utils/ # Evaluation tools (math, science, reasoning)
- README.md


---

## 🔁 System Architecture Diagram

```mermaid
flowchart TD

subgraph Agent_A ["Agent A"]
    A1[Latent State]
    A2[Inner Recursive Loop]
    A1 --> A2 --> A1
end

subgraph Agent_B ["Agent B"]
    B1[Latent State]
    B2[Inner Recursive Loop]
    B1 --> B2 --> B1
end

subgraph Agent_C ["Agent C"]
    C1[Latent State]
    C2[Inner Recursive Loop]
    C1 --> C2 --> C1
end

%% Recursive Links (Outer Links)
A1 -- RecursiveLink --> B1
B1 -- RecursiveLink --> C1
C1 -- RecursiveLink --> A1

%% Hierarchical Layer
subgraph Swarm_Orchestration ["Swarm Orchestration"]
    P[Planner]
    C[Critic]
    S[Solver]
end

P --> C --> S
S --> P

%% MoE Layer
subgraph MoE ["Mixture of Experts"]
    M[Math Expert]
    Co[Code Expert]
    Sc[Science Expert]
    Sum[Latent Summarizer]
end

M --> Sum
Co --> Sum
Sc --> Sum

%% Distillation
Expert[Large Expert Model] -->|Latent Guidance| Small[Small Model]

%% Connections to agents
A1 --> P
B1 --> M
C1 --> Co

