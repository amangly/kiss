# kiss

A KISS (keep It Simple Stupid) skill for coding agents. Solve the current problem with the simplest readable code that fully works.

Use it to build features, simplify existing code, or review a diff. It checks for unnecessary abstractions, unused options, deep nesting, and premature optimization. Existing behavior and required checks stay intact.

## Install

```sh
npx skills add amangly/kiss --skill kiss
```

Choose your coding agent when prompted. Add `-g` to install across projects.

## Use

```text
/kiss simplify this function without changing its behavior
/kiss review this diff for unnecessary abstractions
```

In Codex, use `$kiss` in place of `/kiss`.

The rules target functions of at most 30 lines, cyclomatic complexity of at most 7, and two nesting levels. Exceptions need a concrete requirement or measurement.

Read the full [skill](skills/kiss/SKILL.md).
