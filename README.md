# AI `AGENTS.md` Bootstrap

Turn a repository into a workspace that AI agents can understand quickly and change confidently.

[`AGENTS.bootstrap.md`](AGENTS.bootstrap.md) is a rigorous construction protocol for creating a project-specific `AGENTS.md`. It guides an agent through the repository, connects architecture to real files and symbols, captures verified development workflows, and preserves the implementation knowledge that is usually rediscovered in every new session.

The result is a living operational map: concise enough to consult before a change, detailed enough to locate the right code and avoid repeating known mistakes.

## What it gives your project

- **Fast orientation:** project purpose, maturity, terminology, principles, and sources of truth are clear from the start.
- **A navigable file reference:** every meaningful file gets its own linked subsection with responsibilities, important functions and subparts, callers, dependencies, tests, and common mistakes.
- **Feature-level understanding:** cross-file features are traced from their entry points through their owners, constraints, and focused tests.
- **Reusable debugging knowledge:** recurring error patterns explain their symptoms, causes, safe implementation patterns, and regression checks.
- **Verified workflows:** exact commands for building, running, testing, debugging, packaging, and releasing come from the repository itself.
- **Safer changes:** security, privacy, persistence, compatibility, concurrency, and lifecycle boundaries remain visible beside the code that enforces them.
- **Documentation that stays useful:** task, edit, and commit triggers show when the handbook must evolve with the project.

## How it works

The bootstrap leads an agent through a structured discovery pass before it writes the final handbook:

1. Establish the checked-out repository state and applicable instructions.
2. Identify authoritative documents, source areas, entry points, interfaces, tests, and generated artifacts.
3. Verify executable workflows and trace the real architecture and feature paths.
4. Extract critical contracts, recurring failure modes, and safe development patterns.
5. Replace the bootstrap guidance with verified, project-specific knowledge.
6. Validate links, commands, status labels, and consistency with the source.

This makes the generated `AGENTS.md` evidence-based and specific to the current revision instead of a generic checklist.

## Use it

From the target repository root, copy the bootstrap as `AGENTS.md`:

```sh
cp /path/to/ai-agents-bootstrap/AGENTS.bootstrap.md AGENTS.md
```

Then ask your AI agent to follow the bootstrap completely and replace its protocol text and placeholders with findings from the target repository.

If the file has already been copied under its original name, rename it first:

```sh
mv AGENTS.bootstrap.md AGENTS.md
```

Review the generated handbook together with the code and keep it in the repository root. Independently built or governed subsystems can add nested `AGENTS.md` files for their local rules.

## What the finished handbook covers

The recommended structure includes:

- project mission, non-goals, maturity, and terminology;
- read order and source-of-truth hierarchy;
- collaboration and maintenance rules;
- essential principles and critical implementation contracts;
- architecture and data/control flows;
- a linked, subsection-based file and symbol reference;
- features and recurring development pitfalls;
- interface and test ownership maps;
- build, run, debug, packaging, release, and deployment commands;
- data, security, privacy, migration, and compatibility boundaries;
- shipped behavior, experiments, known gaps, and near-term priorities;
- task-start, handoff, validation, and documentation-update checklists.

The full protocol also scales its source reference to the repository: small projects can document every meaningful file, while large projects can focus on entry points, registries, boundaries, hotspots, and non-obvious owners without losing navigability.

## The quality bar

A useful `AGENTS.md` reflects the checked-out code, links to its evidence, explains why important boundaries exist, and clearly separates current behavior from future plans. It complements the README, tests, architecture decisions, and roadmap by connecting them into one fast-access reference for implementation work.

Start with the [bootstrap protocol](AGENTS.bootstrap.md), let the repository supply the facts, and leave the next agent a codebase it can navigate without starting over.

## License

Released under [CC0 1.0 Universal](LICENSE).
