
# 🌌 boltzmann_ballast: Thermodynamic Agentic Ops Substrate

> *"In a system of high agency, entropy is not a risk; it is a certainty. Stability requires a ballast."*

This `README.md` is designed to be the foundational document for **boltzmann_ballast**. 
It establishes the technical directives, architectural philosophy, and operational protocols 
for your AgentOps substrate, ensuring it integrates seamlessly with the rest of your AntiGravity stack.

***

## 1. Project Overview
`boltzmann_ballast` is the operational nervous system for the autonomous agent fleet. While `tachyon_tongs` provides the firewall and `penumbra_substrate` manages the epistemic memory, `boltzmann_ballast` ensures the **Observability, Orchestration, and Reliability** of the entire swarm.

By treating agent behavior as a thermodynamic system, this project monitors for "semantic heat" (behavioral drift) and provides the "ballast" (stabilization and control) necessary to prevent architectural decay or agentic runaway.

## 2. The Problem: Thermodynamic Decay in AI Swarms
Autonomous agents introduce unique operational challenges that traditional DevOps cannot address:
* **Semantic Drift:** Agents slowly deviate from their original instructions over multi-step tasks ("Boiling the Frog").
* **Execution Entropy:** Non-deterministic tool use leads to unpredictable resource consumption and system state changes.
* **Identity Spoofing:** Determining if a heartbeat or log actually originated from a trusted agent node.
* **Operational Blindness:** The difficulty of correlating thoughts and actions across multiple repositories and devices.

## 3. The Ballast Architecture
`boltzmann_ballast` implements a three-layer governance model to manage agentic entropy.



### A. Accretion Axis (Telemetry & Logging)
The centralized "sink" for all telemetry. It collects immutable traces of every thought, tool call, and system interaction.
* **Mechanism:** PQC-signed A2A (Agent-to-Agent) streaming.
* **Key Artifact:** `accretion.log` — A cryptographically anchored ledger of agent history.

### B. Entropy Engine (Monitoring & Analysis)
The analytical core that evaluates agent health using local MLX models.
* **Metrics:** * **Goal Drift Index:** Semantic distance between the current state and the `ROOT_GOAL`.
    * **Action Heat:** Frequency of high-risk tool calls (e.g., `file_delete`, `network_fetch`).
    * **Probabilistic Baselines:** Detecting actions that fall outside the agent's statistical "norm."

### C. Ballast Control (Orchestration & Stability)
The enforcement layer that stabilizes the fleet.
* **Heartbeat Protocol:** Mandates a periodic, signed "Check-In" from every active agent process.
* **Kill-Switch Logic:** Automated "Freeze" or "Quarantine" routines for agents exceeding entropy thresholds.
* **Scaling:** Managing the lifecycle of Lima/Matchlock sandboxes.

## 4. Security & Integrity
This project follows the **Zero-Trust Agentic Operations** standard:
* **PQC Attestation:** Every heartbeat and telemetry packet is signed using **ML-DSA-65 (Dilithium3)** to prevent adversarial spoofing.
* **Local-First / Air-Gapped:** All telemetry analysis occurs on local Apple Silicon (M5) to ensure that sensitive operational metadata never leaks to the cloud.
* **Hardware Interlock:** Critical "Ballast" operations (like a global swarm halt) require physical **YubiKey 5C** attestation.

## 5. Ecosystem Integration
`boltzmann_ballast` serves as the data provider for your other security nodes:
1.  **Detection:** `entropy_engine` detects a 30% drift in an agent's objective.
2.  **Reporting:** Telemetry is forwarded to the `Herald` alert system.
3.  **Action:** `singularity_pdp` updates the OPA policy to throttle the agent's capabilities.
4.  **Recovery:** `ballast_control` restarts the agent in a clean `Matchlock` sandbox.

## 6. Operational Interface (Slash Commands)
Manage the fleet via the standardized operator interface:
* `/heartbeat`: View the status and PQC-validity of all active agents.
* `/entropy`: Display a real-time "Heat Map" of behavioral drift across the swarm.
* `/quarantine [agent_id]`: Immediately move an agent to a restricted, non-networked sandbox.
* `/purge-logs`: Cryptographically shred telemetry data older than the retention period.

## 7. Development Roadmap
* **Phase 1:** Implementation of the `accretion_axis` logging daemon and SQLite state ledger.
* **Phase 2:** Integration of PQC-signed heartbeats for In-Band agents.
* **Phase 3:** Development of the MLX-based Behavioral Baseline generator.
* **Phase 4:** Real-time entropy dashboard (Next.js/Tailwind) for visual swarm oversight.

***
*"Stability through vigilance. Reliability through math."*

