# Prompt Engineering Templates

![Prompt Engineering Templates](https://img.shields.io/badge/LLM-Prompt%20Engineering-blueviolet?style=flat-square)

> **A comprehensive, open-source collection of prompt templates and instruction sets for effective interaction with Large Language Models (LLMs) across software, data, infrastructure, and prompt engineering domains.**

---

## Quickstart

1. **Browse** the [Instruction Sets](#instruction-sets) below or in the repo folders.
2. **Copy** the relevant XML or Markdown file for your use case.
3. **Paste** it at the start of your LLM session (ChatGPT, Copilot, etc.).
4. **Ask** your questions or describe your task—get better, more focused results!

---

## Repository Structure

```
MetaPrompts/   # Meta-level prompt engineering and orchestration
Prompts/       # General prompt templates (e.g., planning)
System/        # Domain-specific instruction sets (Codex, Copilot, OpenAI, Planner)
README.md      # This file
```

---

## What’s Inside?

### Why Use This Repo?

- **Battle-tested templates** for LLMs—get better results, faster.
- **Domain coverage:** software, data science, MLOps, DevOps, prompt engineering, and more.
- **Meta-prompting tools** for advanced orchestration and planning.
- **Open source, extensible, and community-driven.**

---

## Instruction Sets

### Software Engineering

- **codex.xml** — General instruction set for expert software engineering assistance. Use for comprehensive programming support across languages and paradigms.
- **codex-backend.xml** — Backend engineering: API design, database optimization, server architecture.
- **codex-frontend.xml** — Frontend development: UI/UX, responsive design, modern frameworks.
- **codex-fullstack.xml** — End-to-end application development, bridging frontend and backend concerns.

### Data & Machine Learning

- **codex-datascience.xml** — Data analysis, visualization, and statistical modeling workflows.
- **codex-mlops.xml** — Machine learning operations, model deployment, and production ML systems.

### Infrastructure

- **codex-devops.xml** — Infrastructure as code, CI/CD pipelines, and cloud platform management.

### Meta-Prompting & Prompt Engineering

- **MetaPrompts/meta-prompt.xml** — Meta-instruction set for advanced prompt engineering strategies.
- **MetaPrompts/meta-system.md** — System-level meta-guidance for prompt engineering and LLM orchestration.
- **MetaPrompts/prompt-engineer.xml** — Templates and instructions for prompt engineering roles and workflows.
- **Prompts/plan-mode.xml** — Template for planning, step-by-step reasoning, and structured task decomposition.
- **System/Planner/system_planner.xml** —
  - **Comprehensive system-planner for feature/blueprint design and task decomposition.**
  - **Key Features:**
    - Four-phase lifecycle: Discussion, Design, Iteration, Plan Splitting
    - Ultra-think and deep-think directives for rigorous, multi-step reasoning
    - Output files: `{feature_name}_plan.md` (detailed plan) and `{feature_name}_steps.md` (split, atomic tasks)
    - Explicit success criteria and completeness checklist (Goals, Success Criteria, Stakeholders, Requirements, Glossary, Assumptions, Dependencies, Data Schemas, Algorithms, API Contracts, Error Handling, Risks, Security, Performance, Ops, Metrics, Citations)
    - Output format: YAML front-matter, structured sections, split-step example
    - Strict phase control: never advance without explicit user cue; always clarify ambiguity
    - Private notes protected and excluded from downstream output unless authorized
    - Professional, precise, and systematic tone
  - **Example Output Format:**
    ```markdown
    # Project Plan: {feature_name}

    ---

    version: 0.1
    date: YYYY-MM-DD
    authors: ["user", "assistant"]
    changelog:

    - YYYY-MM-DD: v0.1 - Initial draft creation

    ---

    ...
    ```
  - **Split-Step Example:**
    ```markdown
    ### Task 1 - Set Up Project Skeleton

    - **Instructions:** Create the directory structure and boilerplate files described in § 2.2 of the plan.
    - **Verification Criteria:** All listed directories and empty files exist.

    ### Task 2 - Implement Data Parsing Module

    - **Instructions:** Write `parse_input()` to handle the input format in § 2.1, covering edge cases from § 6.
    - **Verification Criteria:** Unit tests pass for valid and invalid samples.
    ```

### LLM-Specific Guidance

- **System/Copilot/copilot-instructions.md** — Guidelines for effective pair programming with GitHub Copilot, including best practices and optimization techniques.
- **System/OpenAI/open-ai-swe.md** — Specialized prompts and instructions for OpenAI software engineering tasks.
- **System/Codex/codex-prime.md** — Prime instruction set for advanced coding scenarios and expert-level assistance.

---

---

## 🛠️ Usage

1. **Identify** the instruction set or template that matches your current task or domain.
2. **Copy** the content of the relevant XML or Markdown file.
3. **Paste** it at the beginning of your conversation with an LLM (e.g., ChatGPT, Copilot, etc.).
4. **Describe** your specific questions, requirements, or tasks.

>  **Tip:** For best results, always choose the instruction set that most closely aligns with your intended use case.

---

## Contributing

We welcome contributions from the community!

1. **Fork** the repository
2. **Create** a feature branch
3. **Add or update** prompt templates or documentation
4. **Submit** a pull request with a clear description of your changes

**Guidelines:**

- Please ensure your contributions are well-documented and follow the existing organizational structure.
- Add examples and usage notes where possible.
- Be kind and constructive in discussions.

---

## License

This repository is free to use. See individual files for any additional licensing details.

---
