# ADK Master Gateway (GEMINI.md)

## Purpose
This MCP server implements the **Google ADK "Sidecar" (A2A) Architecture**. It acts as the central orchestrator (Master Gateway) that delegates complex reasoning tasks to specialized autonomous sidecar agents.

## Usage for Agents
- Use `adk_delegate_task` when you identify a high-level mission that requires a specialized sub-agent (e.g., Security, Lifecycle, Engineering).
- Use `adk_get_ecosystem_health` to check if all sidecars are online and ready to accept missions.

## Strategic Role
This is the "Brain" of the ecosystem. It manages the lifecycle and communication between different specialized MCPs.
