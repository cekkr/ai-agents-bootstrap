# AI `AGENTS.md` Bootstrap

A rigorous bootstrap protocol for creating or repairing a repository's root [`AGENTS.md`](AGENTS.bootstrap.md). It helps AI agents build a current, high-signal operational reference: project purpose, authoritative sources, architecture, ownership, commands, contracts, test coverage, and maintenance rules.

This repository contains a bootstrap, not a generic `AGENTS.md` to copy unchanged. The resulting handbook must be based on an inspection of the target repository and its checked-out revision.

## Use it

1. Copy [`AGENTS.bootstrap.md`](AGENTS.bootstrap.md) into the root of the target repository.
2. **Rename the copied file to `AGENTS.md`.** Do not leave it as `AGENTS.bootstrap.md`.
3. Follow the mandatory discovery pass in the document before writing project-specific content.
4. Replace generic guidance and placeholders with verified facts, paths, commands, contracts, and tests from that repository.
5. Validate local links, commands, consistency with authoritative documents, and the final diff.

For example, from the target repository root:

```sh
cp /path/to/ai-agents-bootstrap/AGENTS.bootstrap.md AGENTS.md
```

Or, if the bootstrap has already been copied into the target repository:

```sh
mv AGENTS.bootstrap.md AGENTS.md
```

## What the finished `AGENTS.md` should provide

- A clear project mission, non-goals, maturity, and source-of-truth order.
- Concrete principles and critical implementation contracts, including dangerous boundaries and their tests.
- A clickable ownership map for source, interfaces, tests, generated artifacts, and nested instructions.
- Verified build, run, test, debug, packaging, and release workflows.
- Clear distinctions between shipped behavior, experiments, known gaps, and plans.
- Task-by-task, edit-by-edit, and commit-by-commit documentation maintenance rules.

## What it is not

The bootstrap is not a README replacement, changelog, backlog, architecture dump, or place for credentials. It must not make up facts, commands, configuration, test counts, or implementation status.

## License

Released under [CC0 1.0 Universal](LICENSE).
