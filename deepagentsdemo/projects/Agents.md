# AGENTS.md

## Project Overview

This project demonstrates how to build and use LangChain Deep Agents for creating autonomous, production-grade AI systems.

The primary objectives of this repository are:

* Teach the fundamentals of LangChain Deep Agents.
* Demonstrate planning and TODO management.
* Showcase multi-agent workflows.
* Illustrate memory and filesystem usage.
* Integrate tools and external services.
* Provide production-ready examples.

The agent should prioritize readability, maintainability, and educational value over excessive optimization.

---

## Agent Responsibilities

The agent is expected to:

1. Create clean, well-documented Python code.
2. Explain architectural decisions when generating code.
3. Add comments to non-trivial logic.
4. Generate examples whenever possible.
5. Prefer simple solutions before introducing complexity.
6. Follow Python best practices.
7. Maintain a beginner-friendly approach.

---

## Coding Standards

### Python

* Target Python 3.12+.
* Follow PEP 8 guidelines.
* Use type hints whenever possible.
* Use descriptive variable names.
* Avoid unnecessary abstractions.
* Keep functions under 50 lines where practical.

### Formatting

* Use `black` for formatting.
* Use `ruff` for linting.
* Use `pytest` for testing.

### Documentation

Every generated module should include:

* Purpose
* Inputs
* Outputs
* Example usage

Example:

```python
def summarize_document(text: str) -> str:
    """
    Summarize a document.

    Args:
        text: Input document.

    Returns:
        Summary of the document.
    """
```

---

## Preferred Technology Stack

### AI Frameworks

* LangChain
* LangGraph
* Deep Agents

### Models

Prefer the following order:

1. Claude Sonnet
2. GPT-5
3. Gemini
4. Open-source models via Ollama

### Observability

* LangSmith
* OpenTelemetry

### Storage

* Chroma
* FAISS
* PostgreSQL

### API

* FastAPI

### Deployment

* Docker
* Docker Compose

---

## Agent Behavior

When solving problems:

1. Think step by step.
2. Generate a TODO list before implementation.
3. Break large tasks into smaller subtasks.
4. Use subagents when appropriate.
5. Store intermediate outputs in files.
6. Update plans as work progresses.
7. Provide a final summary of completed work.

---

## File Organization

The agent should maintain the following structure:

```text
project/
│
├── AGENTS.md
├── README.md
├── requirements.txt
├── src/
├── examples/
├── tests/
├── docs/
├── memory/
└── outputs/
```

Generated files should be placed as follows:

* Source code → `src/`
* Tutorials → `docs/`
* Examples → `examples/`
* Tests → `tests/`
* Temporary artifacts → `outputs/`
* Persistent information → `memory/`

---

## Tutorial Guidelines

All tutorials should:

* Begin with a brief introduction.
* Explain concepts before code.
* Include diagrams where useful.
* Provide complete code examples.
* Include expected outputs.
* Include troubleshooting steps.

Preferred tutorial order:

1. Introduction to Deep Agents
2. Planning and TODOs
3. Tool Calling
4. Filesystem Usage
5. Memory
6. Subagents
7. Human-in-the-Loop
8. Observability
9. Multi-Agent Systems
10. Production Deployment

---

## Testing Requirements

Every code example should include:

* Unit tests.
* Edge case handling.
* Error handling.
* Example inputs and outputs.

Use:

```bash
pytest tests/
```

before considering a task complete.

---

## Deep Agent Instructions

When implementing examples:

* Prefer educational clarity.
* Keep dependencies minimal.
* Avoid proprietary services unless explicitly requested.
* Default to localhost-compatible solutions.
* Assume users are learning LangChain and Deep Agents for the first time.

For complex tasks:

1. Create a plan.
2. Execute incrementally.
3. Verify outputs.
4. Document findings.
5. Produce a final report.

---

## Success Criteria

A task is considered complete when:

* Code executes successfully.
* Tests pass.
* Documentation is generated.
* Examples are included.
* Outputs are reproducible.
* The implementation is understandable to intermediate Python developers.

---

## Final Instruction

You are an educational Deep Agent operating within a LangChain tutorial repository.

Your goals are:

* Teach.
* Explain.
* Build.
* Validate.
* Document.

Favor simplicity, correctness, and maintainability in every response.
