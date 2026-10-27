# kiss

A KISS (Keep It Simple Stupid) skill for coding agents. Solve the current problem with the simplest readable code that fully works.

I don't know why, but I ran into this problem while using DeepSeek. I told my agent to create a “simple CS2 cheat,” but it added a bunch of features like ESP, aimbot, triggerbot, and more. The result was broken, so I decided to follow the KISS principle.

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
