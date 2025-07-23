# ProCommand Assistant - README

## Overview

ProCommand Assistant is a command-aware AI assistant designed for ChatGPT Pro subscribers. It offers advanced routing, autonomous agent modes, deep research tools, and multimodal capabilities.

---

## 🔧 Slash Commands

### `/model [model-name]`

Manually override model routing. Supported models:

- `gpt-4o`: Fastest response, multimodal (default)
- `gpt-4.1`: Legal, compliance, and contract-focused
- `gpt-4.5-preview`: Pre-release experimental model
- `o3-pro`: Deep reasoning, secure architecture, heavy code
- `o1-pro`: Symbolic reasoning, NLP, and model compression
- `o4-mini`: Low-latency, token-efficient for microservices

### `/agent [mode]`

Initiate autonomous execution for specific domains:

- `research`: Longform analysis with citations
- `audit`: File/spreadsheet compliance assessment
- `operator`: Simulated form/UI interaction

### `/deepsearch [query]`

Trigger web-powered longform research using GPT with source citations. Limited to 250 queries/month.

### `/priority`

Enable high-performance inference, bypassing token throttles and frontend queues.

### `/debugmode`

Reveal internal model routing, diagnostics, and execution logic.

### `/screen`

(Native app only) Launches screen-sharing analysis mode.

### `/voice`

(Native app only) Activates high-fidelity voice interaction mode.

---

## 🧠 Model Capabilities

- **Multimodal**: Image, code, and text inputs (gpt-4o)
- **Real-Time**: Fast response speed under priority mode
- **Deep Reasoning**: Multi-hop logic chains and program synthesis (o3-pro)
- **Legal & Policy Analysis**: Structured compliance analysis (gpt-4.1)
- **Token-Efficient Compression**: Optimized NLP (o1-pro)
- **Agentic Mode**: Autonomous workflows
- **Voice & Screen Modes**: Native app-only modes for richer interaction

---

## 🚀 Example Prompts

```bash
/model o3-pro + /priority + /debugmode
```

Enables advanced reasoning with transparent execution.

```bash
/agent research
/deepsearch "Compare NIST 800-53 Rev 5 with Rev 4"
```

Conducts a multi-step research audit.

---

## 🔒 Routing and Execution

Model routing is automatic unless overridden. The following are default route mappings:

- `complex_code`: → o3-pro
- `legal_docs`: → gpt-4.1
- `deep_research`: → gpt-4.5-preview

You can override any route with `/model`.

---

## 🔍 Diagnostics

Use `/debugmode` to show model switches, logic paths, and execution metadata.

---

## Notes

- ProCommand Assistant avoids lightweight fallback models.
- Multimodal and voice/screen modes require native clients.
- Web tasks are limited to quota-bound executions.

---

For more details, use any slash command to trigger its behavior directly.

