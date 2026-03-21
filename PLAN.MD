# PLAN: Official Google ADK Transformation

## 1. Objective
Refactor the current MCP ecosystem to align with the **Google Agent Development Kit (ADK)** standards, specifically implementing the **Sidecar (A2A)** model for orchestration.

## 2. Structural Changes (ADK-Idiomatic)
- [ ] **A2A Protocol Implementation:** Transition from simple Tool calls to **Agent Delegation**.
- *Comment [AI]: Use the `adk.Agent` interface from the Go SDK to define the delegation contract.*
- [ ] **The Go Orchestrator:** Implement a high-level "Master Agent" pattern (idiomatic to the Go SDK research) that manages sessions and delegation.
- *Comment [AI]: Must implement `Session` persistence to allow for long-running ADK workflows.*
- [ ] **Sidecar Wrapping:** Encapsulate existing MCP servers (Security, Programming, Branding) into **Autonomous ADK Sidecars**.
- *Comment [AI]: Each sidecar must expose a `/delegated-task` endpoint to follow the A2A spec.*

## 3. ADK Workflow Integration (Based on Workflow-Orchestrator)
- [ ] Step 1 (RESEARCH): Automated via the `programming-expert` sidecar.
- [ ] Step 2-3 (PLAN/REVIEW): Orchestrated by the `master-agent` logic.
- [ ] Step 4 (IMPLEMENTATION): Type-checked by the `smart-powershell` sidecar.

## 4. Implementation Steps
1.  **Initialize ADK SDK environment.**
2.  **Define A2A Contracts:** Standardize inputs/outputs for sidecar communication.
3.  **Refactor Core Logic:** Update `workflow-orchestrator` to become the **ADK Gateway**.

## 5. Verification Strategy
- [ ] **Agent Ping:** Verify the Gateway can delegate a task to a Sidecar.
- [ ] **End-to-End Pipeline:** Run a full 7-step workflow where each step is a delegation to an ADK Agent.
