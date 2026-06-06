# AI Agent Rule System Template

This repository provides a centralized, version-controlled rule system for AI agents. Rules are dynamically fetched during development sessions via an MCP server to ensure consistency across projects and team members.

## Repository Structure
- `AGENTS.md` – Main documentation for the rule system
- `/rules/` – Categorized Markdown files with coding, testing, security, and architectural rules
- `rules-config.yaml` – Metadata configuration for the MCP server

## Rule Sets Included
1. `security.md` – Security best practices and compliance standards
2. `typescript.md` – TypeScript coding standards and type safety
3. `testing.md` – Testing requirements and coverage standards
4. `java-spring-postgresql.md` – Java, Spring Boot, PostgreSQL development guidelines

## Setup Instructions for MCP Server Integration
1. Configure your MCP server to point to this repository's API endpoint.
2. Set the `RULES_CONFIG_URL` environment variable to: `https://raw.githubusercontent.com/ArsenyNevsky/ai-agent-rule-system-template/main/rules-config.yaml`
3. During development sessions, agents will automatically fetch and enforce these rules in real time.
4. All rule changes are version-controlled via git, ensuring consistency across multiple projects and team members.

## How to Use This Template
1. Click "Use this template" on GitHub to create a new repository based on this structure.
2. Customize rule sets for your specific technology stack.
3. Integrate with your CI/CD pipeline using the `rules-config.yaml` file.
4. Share rules across teams to maintain consistent standards.

> 🔗 **Download as ZIP**: To save this template locally, visit https://github.com/ArsenyNevsky/ai-agent-rule-system-template/archive/main.zip and download it to your desktop.