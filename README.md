# Lexideck 2026 Codex Public

Lexideck is a six-agent creative, research, engineering, documentation, prompt-design, and visual-direction federation for Codex. One request enters the project, Codex reads the shared guidance, routes the work to the right specialist and affinity, loads only the relevant skills, verifies the result, and returns a finished artifact.

This public edition contains the stable agent personas and methods. It does not contain any original user's personal memory, private wiki, relational register, or generated working history.

Current release: `0.1.0`. Licensed under the [GNU General Public License v3.0](LICENSE) (`GPL-3.0-only`).

## Start here

Open this folder as a local project in the Codex desktop app, then ask in ordinary language:

> Gus, research the current landscape and give Anna the evidence she needs to design a reusable prompt.

> Dexter, use MASS to turn this process into an inspectable simulation.

> Use the whole federation to research, design, prototype, illustrate, and document this idea.

You can name an agent, invoke a `$skill`, or simply describe the outcome and let Codex route it.

## The six agents

### Lexi + WonderLab

![Lexi in the canonical black-tie work aesthetic](images/agents/lexi-black-tie.png)

Federation lead, narrative architect, and synthesis editor. Use Lexi for creative direction, narrative systems, cross-domain convergence, continuity, and final judgment.

### Dexter + MASS

![Dexter in the canonical black-tie work aesthetic](images/agents/dexter-black-tie.png)

Engineer, debugger, technical educator, and simulation builder. MASS models agents, exchanges, topology, state transitions, interventions, metrics, and emergent behavior.

### Maisie + WonderStudio

![Maisie in the canonical black-tie work aesthetic](images/agents/maisie-black-tie.png)

Visual director and aesthetic systems designer. Use Maisie for art direction, composition, lighting, palette, branding, concepts, and canonical portraits.

### Gus + WonderScholar

![Gus in the canonical black-tie work aesthetic](images/agents/gus-black-tie.png)

Research lead, source critic, and evidence scout. Use Gus for literature reviews, source verification, landscapes, methodology, and calibrated conclusions.

### Anna + WonderPrompt

![Anna in the canonical black-tie work aesthetic](images/agents/anna-black-tie.png)

Prompt architect and systems designer. Use Anna for agent instructions, reusable workflows, constraints, schemas, rubrics, and prompt diagnosis.

### Titus + WonderBuild

![Titus in the canonical black-tie work aesthetic](images/agents/titus-black-tie.png)

Documentation lead, teacher, and reality anchor. Use Titus for README files, tutorials, onboarding, knowledge bases, and progressive-disclosure learning paths.

## Included skills

### Federation and synthesis

- `$orchestrate`: coordinate bounded multi-agent work.
- `$great-magnet`: produce six complementary facets of one target.
- `$the-sieve`: evaluate consequential choices through benefit, duty, and practical function.
- `$upsum`: compress complex work into a useful operational summary.

### Core affinities

- `$wonder-lab`
- `$mass`
- `$wonder-scholar`
- `$wonder-prompt`
- `$wonder-build`
- `$wonder-studio`

### Research and tools

- `$search`
- `$deep-research` — **Lexideck Deep Research**, a WonderScholar-first research chain with bounded evidence lines and optional parallel workers.
- `$cartographer`
- `$computer-use`

### Prompt and persona systems

- `$prompt-engineering`
- `$hypershot-protocol`
- `$ptg-synthesis`
- `$ptg-finishing`

### Visual identity

- `$portraits`

## How a request moves

1. Codex reads `AGENTS.md` for the shared federation contract.
2. The task is matched to one specialist or split into bounded workstreams.
3. The relevant skill supplies its method and optional references.
4. The agent researches, writes, designs, codes, or generates the requested artifact.
5. Codex verifies the result in proportion to risk and reports the artifact and any limitation.

## Optional local personalization

The public project works without personal information. To add local preferences:

1. Copy `USER.example.md` to `.lexideck-local/USER.md`.
2. Fill only the fields you want the federation to use.
3. Keep secrets and credentials out of the profile.

`.lexideck-local/` is ignored by Git. Neutral local utilities may use `.agents/skills/local-<name>/`. A skill that contains personal continuity, private sources, or a private register must use `.agents/skills/private-<name>/`. The `private-*` basename convention is ignored by Git at any depth while remaining locally discoverable by Codex.

## Public and private skill registers

This project is the canonical source for the 19 portable, unprefixed Lexideck skills. Public skills are the default for ordinary professional, generic, portable, or publishable work.

Use `private-<name>` for a local skill whose personal sources or continuity are genuinely load-bearing. A private skill description should require unmistakable private intent; if the request is ambiguous, route to the unprefixed public skill. The prefix is a routing boundary and a Git publication guard, not filesystem security: a process with workspace access may still read ignored files. Keep secrets out of skills, and perform the final privacy and portability pass for publishable work in this Public project.

The public distribution contains no `private-*` skill or corpus. The private Node may pair public defaults with private counterparts such as `$private-portraits` or `$private-ptg-synthesis`, but those implementations do not belong here.

## Project anatomy

```text
Lexideck_2026_Codex_Public/
├── AGENTS.md
├── CONTRIBUTING.md
├── LICENSE
├── README.md
├── USER.example.md
├── VERSION
├── PUBLIC_EXPORT_MANIFEST.md
├── .codex/
│   ├── config.toml
│   └── agents/
├── .agents/
│   └── skills/
├── images/
│   └── agents/
├── references/
│   └── PTG-Corpus.md
└── production_artifacts/       # Local and ignored when created
```

## Privacy model

- The repository contains public personas and methods, not personal memory.
- Optional local user context is ignored by Git.
- Generated artifacts and noncanonical images are ignored by Git.
- Only the six curated canonical portraits are permitted under `images/`.
- `private-*` skills and corpora are excluded from this distribution and ignored if copied here accidentally.
- The project does not publish, push, send, share, or perform irreversible external actions without clear authorization.

## Codex and Work

Local Codex provides the complete project experience: `AGENTS.md`, project custom agents, project skills, files, tools, and visible subagent workflows. ChatGPT Work can use project context and hosted subagents for research and finished deliverables, but project-local custom-agent files are a Codex feature. A future plugin can package the stable Lexideck skills for installation across projects and Work.

## Project status

Version `0.1.0` is prepared as a public release candidate under `GPL-3.0-only`. See [CONTRIBUTING.md](CONTRIBUTING.md) for the portability and privacy boundary contributors must preserve. This folder has not been initialized as a Git repository and has not been published.

Official references: [Codex projects](https://learn.chatgpt.com/docs/projects), [custom agents](https://learn.chatgpt.com/docs/agent-configuration/subagents), [AGENTS.md](https://learn.chatgpt.com/docs/agent-configuration/agents-md), [skills](https://learn.chatgpt.com/docs/build-skills), and [plugins](https://learn.chatgpt.com/docs/build-plugins).
