# AI Agent Rule System

This repository provides a centralized, version-controlled rule system for AI agents. Rules are dynamically fetched during development sessions via an MCP server to ensure consistency across projects and team members.

## Rule Structure
- `rules/` directory contains categorized rule sets in Markdown
- `rules-config.yaml` defines metadata and mappings for the MCP server
- Rules are enforced at development time via agent integrations

## Setup Instructions
1. Initialize your project using this template.
2. Configure the MCP server endpoint to point to this repository.
3. Agents will automatically fetch rule sets during session initiation.