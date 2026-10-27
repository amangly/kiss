# kiss

A KISS (Keep It Simple Stupid) skill for coding agents. Solve the current problem with the simplest readable code that fully works.

I asked DeepSeek for a simple CS2 cheat. It added ESP, aimbot, triggerbot, and more, and the result was broken. That's why I built kiss. With the skill, the agent built only ESP, and it worked.

![The DeepSeek session that led me to build kiss](assets/why-kiss.png)

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
