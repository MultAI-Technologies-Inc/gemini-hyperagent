# Gemini Hyperagent Extension

A metacognitive framework for the Gemini CLI that enables agents to autonomously analyze their own performance and iteratively optimize their system instructions.

## 🚀 Overview

The Hyperagent extension implements a "self-evolution" loop. It allows an AI agent to monitor its own telemetry, identify bottlenecks, and rewrite its core operating protocols (**GEMINI.md**) to improve its efficiency and reasoning over time. This framework is project-agnostic and can be integrated into any workspace.

## 🛠 Features

- **Autonomous Evolution**: Triggers an iterative loop where the agent reviews its own performance data and "mutates" its instructions for the next epoch.
- **Performance Archiving**: Maintains an immutable record of every generation, including its instructions and associated fitness scores.
- **Safety-First Mutation**: Includes a "Splicing" mechanism that only updates mutable sections of the system instructions, preserving core directives and system integrity.
- **Autonomous Tooling Development**: Agents can identify recurring pain points and build their own helper scripts in `hyperagent/tools/`. These are tracked as candidate features for future core updates.
- **Telemetry-Driven Insights**: Provides a structured audit of performance metrics and bottlenecks.

## 📥 Installation

```bash
gemini extensions install https://github.com/MultAI-Technologies-Inc/gemini-hyperagent
```

## ⌨️ Commands

| Command | Description |
| :--- | :--- |
| `/hyperagent:init` | Scaffolds the Hyperagent framework in the current project directory. |
| `/hyperagent:analysis` | Audits current state and analyzes performance telemetry. |
| `/hyperagent:evolve` | Triggers a metacognitive rewrite of the project's instructions. |
| `/hyperagent:help` | Displays detailed information about the Hyperagent framework and its components. |

## 🏗 Framework Components

When initialized, the following files are deployed to the `hyperagent/` directory:

- **`GEMINI.md`**: The system "DNA." Contains the instructions the agent follows, with a dedicated `MUTABLE` section for evolution.
- **`hyperagent-evolve.py`**: The orchestrator that manages the evolution cycle and archives snapshots.
- **`mutate-dna.py`**: The safe-splicer that updates the `GEMINI.md` file without corrupting its structure.

## ⚖️ License

Released under the BSD 3-Clause License. Copyright (c) 2026 MultAI Technologies Inc.
