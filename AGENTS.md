# NeuroVerilog — Agent Guidelines

This file tells AI agents how to work on this codebase.

## Project purpose

NeuroVerilog is a **ready-to-use agent for engineers to write Verilog code**. The goals are:

- **RAG** (Retrieval-Augmented Generation) for Verilog knowledge and examples
- **MAS** (Multi-Agent System) for orchestration and specialized roles
- **Easy API** for integration and automation

## What to do

- **Structure**: Keep RAG, MAS, and API concerns separable so each can evolve and be tested independently.
- **Increments**: Prefer small, working steps (e.g. a minimal RAG–agent–API flow) before larger refactors or new subsystems.

## What to avoid

- Don’t hardcode API keys or secrets; use env vars or config.
- Don’t mix Verilog style with unrelated languages or tooling unless the project explicitly adopts them.
- Don’t add large dependencies without aligning with the current plan (see README).

## Conventions

- **Language**: Use **English** for code, comments, commit messages, and docs unless the user asks otherwise.
- **Code**: Prefer clear names, minimal coupling, and tests for non-trivial logic (RAG, MAS, API).

If you’re unsure about scope or design, ask the user before making large changes.
