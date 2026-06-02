# everton-ai-agent-kit 🤖🚀

[![Java](https://img.shields.io/badge/Java-17%2B-ED8B00?style=for-the-badge&logo=java&logoColor=white)](https://www.oracle.com/java/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-6DB33F?style=for-the-badge&logo=spring&logoColor=white)](https://spring.io/projects/spring-boot)
[![Gemini](https://img.shields.io/badge/AI-Gemini%20CLI-4285F4?style=for-the-badge&logo=google-gemini&logoColor=white)](https://ai.google.dev/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)

**everton-ai-agent-kit** is a professional-grade Natural Language AI Harness (NLAH) designed to transform standard AI interactions into a high-performance, multi-agent engineering system. Specialized for **Java/Spring Boot** ecosystems and **DevOps** automation, it provides a structured framework for building, reviewing, and deploying production-ready software.

---

## 🏛️ Architecture: The Multi-Agent Ecosystem

The framework operates on a **Maestro-Persona** architecture. It doesn't just "chat"; it orchestrates a team of specialized agents, each with its own identity, playbook, and constraints.

### 🧠 The Core Components

| Component | Description |
| :--- | :--- |
| **Maestro** | The conductor. Orchestrates personas, manages session memory, and is the sole interface to the user. |
| **Personas** | Specialized identities (Architect, Coder, Reviewer, DevOps) that handle specific phases of the lifecycle. |
| **Skills** | Reusable, tool-specific procedures (e.g., `github-portfolio`, `code-sec-review`, `task-tracking`). |
| **Rules** | The "law" of the system. Divided into **Commandments** (absolute), **Edicts** (authoritative), and **Counsel** (guidance). |

---

## 👥 Meet Your AI Engineering Team

| Persona | Role | Focus |
| :--- | :--- | :--- |
| **Maestro** | **Orchestrator** | Intent parsing, delegation, and quality gate management. |
| **Architect** | **Strategist** | System design, API definitions, and implementation planning. |
| **Coder** | **Implementer** | High-fidelity Java/Spring code generation following clean architecture. |
| **Reviewer** | **Quality Gate** | Adversarial review, security audits, and coherence checks. |
| **DevOps** | **Infrastructurist** | Dockerization, CI/CD pipelines, and runtime optimization. |
| **Contextualizer**| **Librarian** | Maintaining codebase knowledge and technical documentation. |

---

## 🛠️ Specialized for Java & Spring Boot

Unlike general-purpose prompts, this kit includes **Edicts** specifically tuned for modern Java engineering:
- **`java-clean-api.md`**: Enforces RESTful best practices and DTO patterns.
- **`spring-boot-architecture.md`**: Mandates Service-Repository patterns and proper dependency injection.
- **`github-professional.md`**: Ensures your portfolio looks like it was built by a Senior Engineer.

---

## 🚀 Installation & Setup

### 1. Integrate into your Project
Clone the kit into a hidden directory within your project:

```bash
cd /your/java-project
git clone https://github.com/evertonrpinheiro/everton-ai-agent-kit.git .agents
```

### 2. Symlink the Entrypoint
Create a symbolic link to make the framework discoverable by the AI:

```bash
# Windows (PowerShell)
New-Item -ItemType SymbolLink -Path "AGENTS.md" -Target ".agents/AGENTS.md"

# Linux/macOS
ln -s .agents/AGENTS.md AGENTS.md
```

### 3. Boot with Gemini CLI
Launch your Gemini CLI and issue the activation command:

```text
Please comply with AGENTS.md.
```

---

## 💻 Usage & Workflow

Once booted, the **Maestro** takes control. You simply provide the intent, and the framework handles the rest:

### Typical Flow
1. **User**: "I need a REST API for managing library books."
2. **Maestro**: Parses intent and dispatches **Architect**.
3. **Architect**: Designs the entities, repositories, and services.
4. **Reviewer**: Validates the plan against `spring-boot-architecture.md`.
5. **Coder**: Implements the code.
6. **Reviewer**: Performs a `code-sec-review`.
7. **Maestro**: Delivers the completed, verified implementation.

### Example Prompts
- `"Implement a Spring Boot REST API for a task manager with PostgreSQL."`
- `"Optimize our Dockerfile for a multi-stage build using Temurin JRE."`
- `"Run a security audit on the current auth module."`
- `"Package this project for my GitHub Portfolio."`

---

## 📈 Roadmap

- [ ] **Spring AI Integration**: Native support for building AI-powered Java apps.
- [ ] **Kubernetes Skills**: Automated Helm chart generation and K8s deployment.
- [ ] **Advanced Testing**: Automated Testcontainers setup for integration tests.
- [ ] **Interactive Dashboard**: (Future) Visual representation of agent tasks and status.

---

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.

---

<p align="center">
  Built with ❤️ for the Java & AI Community by <b>Everton</b>.
</p>
