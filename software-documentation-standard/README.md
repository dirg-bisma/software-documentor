# Software Documentation Standard Skill

A complete, production-ready, reusable AI skill designed to help generate, review, improve, maintain, validate, and trace complex software project documentation.

## Overview
This repository provides a rigorous framework for software documentation, spanning the complete lifecycle from Business Requirements to Technical Design. It is tool-agnostic and designed to be used across ChatGPT, Claude, Antigravity, and other AI coding assistants.

## Structure
- **SKILL.md**: The core AI instruction file.
- **references/**: Detailed rules and standards for documentation.
- **templates/**: Markdown templates for every document type.
- **examples/**: A full suite of documentation examples for a Multi-Property Hotel Platform.

## Usage
Provide the `SKILL.md` to your AI assistant along with the project context. The AI will adopt the personas of Senior Business Analyst, Product Manager, System Analyst, Solution Architect, Technical Writer, and QA Analyst to guide you through the documentation process.

### Example Prompts
- **Generate BRD**: "Using the software-documentation-standard skill, create a BRD for a new multi-tenant SaaS application."
- **Review Document**: "Review this attached PRD based on the software-documentation-standard guidelines and identify any critical issues."
- **Traceability**: "Generate a Traceability Matrix for the requirements defined in the BRD and SRS."

See the [SKILL.md](SKILL.md) for full details on modes, principles, and the generation workflow.
