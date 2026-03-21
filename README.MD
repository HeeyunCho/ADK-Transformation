# ADK Master Gateway: Google A2A Sidecar Environment

This project implements the official **Google Agent Development Kit (ADK)** architecture, transforming a fragmented MCP toolset into a unified **Agent-to-Agent (A2A)** ecosystem.

## 🧠 The Sidecar Model
In this environment, reasoning is decoupled from execution. The **ADK Master Gateway** acts as the primary orchestrator, delegating complex missions to autonomous sidecar agents.

## 🛠️ Integrated ADK Agents
- **SECURITY Sidecar**: Powered by `check-security`.
- **LIFECYCLE Sidecar**: Powered by `workflow-orchestrator`.
- **ENGINEERING Sidecar**: Powered by `programming-expert`.
- **BRANDING Sidecar**: Powered by `github-portfolio-manager`.

## 🚀 How to use
The primary tool for interaction is `adk_delegate_task`.

```typescript
// Example: Delegating a portfolio sync task
mcp_adk_master_gateway_adk_delegate_task({
  agentRole: "BRANDING",
  taskDescription: "Sync all local engineering projects to GitHub and update the profile README."
})
```

## ✅ Verification & Health
Use `adk_get_ecosystem_health` to verify that all sidecar agents are connected and operational.

---
*Developed by Heeyun Cho's Professional Portfolio Suite following Google ADK Standards.*
