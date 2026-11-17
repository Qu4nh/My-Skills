# Agent Skills

A collection of reusable skills for AI agents. Each skill provides instructions and workflows for a specific kind of task.

## Structure

```text
skills/
└── <skill-name>/
    ├── SKILL.md
    └── ... supporting resources
```

Each skill lives in its own directory under `skills/`. Its `SKILL.md` describes its purpose, when to use it, and how to carry out the work.

## Usage

Choose a skill and copy its directory to the location supported by your agent. Keep its supporting resources together. Installation and invocation depend on the agent you use.

Instructions and bundled examples are written in English. Skills follow the user's requested language, or the conversation language when clear, and otherwise default to English. Course materials, notation, and learning goals come from the user rather than a particular country or curriculum.

## Adding a skill

Create a directory under `skills/` with a descriptive name, a `SKILL.md`, and any resources the workflow needs. Keep each skill focused on a specific purpose.
