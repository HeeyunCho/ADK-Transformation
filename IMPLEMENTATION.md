# IMPLEMENTATION: ADK Master Gateway

## Overview
The ADK Master Gateway is built using the Model Context Protocol (MCP) SDK. It manages a registry of "Sidecar Agents" and provides tools for task delegation.

## Tools (Methods)

### 1. `adk_delegate_task`
**Description**: Delegates a task to a sidecar agent.
- **Parameters**:
  - `agentRole` (enum): `SECURITY`, `LIFECYCLE`, `ENGINEERING`, `BRANDING`.
  - `taskDescription` (string): The mission description.
- **Returns**: A confirmation message showing delegation status.

### 2. `adk_get_ecosystem_health`
**Description**: Monitors the status of registered sidecars.
- **Returns**: A list of sidecars and their current status (e.g., 🟢 ACTIVE).

## Protocol
Uses a simulated **A2A (Agent-to-Agent)** protocol for communication. In this implementation, it's an emulation layer that maps roles to specific MCP server names.
