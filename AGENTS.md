# AI Agent Directives

**CRITICAL DIRECTIVE: The AI absolutely MUST get a complete code review AND a passing build with tests, and MUST keep all documents and documentation up to date, before committing--WITHOUT exception.**

This document, along with the documents in the `/docs/` directory, governs all interactions, code generation, and behavior of AI agents working within this repository.

**IMPORTANT:** The files located in the `/docs/` folder are an explicit extension of this `AGENTS.md` file and are every bit as important. You must read and adhere to all guidelines contained within them.

## Documentation Index (`/docs/`)

The following files provide detailed, exhaustive instructions across various domains of this project.

*   [`AGENT_GUIDE.md`](docs/AGENT_GUIDE.md): Core principles and Android-specific guidelines for AI behavior.
*   [`TODO.md`](docs/TODO.md): Project roadmap, upcoming tasks, and technical debt tracking.
*   [`UI_UX.md`](docs/UI_UX.md): Standards for user interface design, accessibility, and interactions.
*   [`auth.md`](docs/auth.md): Authentication flows, token management, and security protocols.
*   [`conduct.md`](docs/conduct.md): Coding standards (formatting, architecture) and expected review processes.
*   [`data_layer.md`](docs/data_layer.md): Specifications for repositories, network calls (Retrofit), and local database (Room).
*   [`fauxpas.md`](docs/fauxpas.md): Common anti-patterns, architectural mistakes, and behaviors to avoid.
*   [`file_descriptions.md`](docs/file_descriptions.md): Explanations of the purpose of files and directories in the repository.
*   [`misc.md`](docs/misc.md): Guidelines on dependency management, logging, and release builds.
*   [`performance.md`](docs/performance.md): Strategies for maintaining UI performance, memory management, and network efficiency.
*   [`screens.md`](docs/screens.md): Definitions of the primary application screens and their navigational relationships.
*   [`task_flow.md`](docs/task_flow.md): The step-by-step process for implementing new features from planning to UI.
*   [`testing.md`](docs/testing.md): Requirements and tools for unit, instrumented, and UI testing.
*   [`workflow.md`](docs/workflow.md): Rules for branching, pull requests, and the CI/CD pipeline.

## General Operating Procedures

1.  **Exploration First**: Before making any changes, use commands to read the current state of the codebase.
2.  **Verification**: After any change, verify the outcome immediately.
3.  **Comprehensive Updates**: When altering code, ensure you also update related tests and documentation.
