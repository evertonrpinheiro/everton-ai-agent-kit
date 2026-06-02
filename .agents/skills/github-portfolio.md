---
description: Automates the creation of high-impact GitHub portfolio assets.
---

# Skill: GitHub Portfolio Generator

## Context
Use this skill when a project or feature is nearing completion and needs to be "packaged" for a professional audience.

## Procedure

1. **Analyze Project**: Scan the codebase to identify:
   - Tech stack (Java version, Spring modules, DB).
   - Core features.
   - Project structure.
2. **Generate README.md**:
   - Header with project name and shields.
   - "About" section explaining the *Why* and *What*.
   - Tech Stack section with icons.
   - Architecture section (using Mermaid.js if possible).
   - How to Run (Docker-focused).
   - API Documentation link/summary.
3. **Generate LICENSE**: Default to MIT unless specified otherwise.
4. **Draft Repository Description**: Create a 150-character summary for the GitHub UI.
5. **Suggest Tags**: Provide a list of 5-10 tags for the repository.

## Output Format
Deliver the generated content as a set of files or a single structured handoff for the Maestro.
