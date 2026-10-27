# kiss

A KISS (Keep It Simple Stupid) skill for coding agents. Solve the current problem with the simplest readable code that fully works.

I used [palepale-rs](https://github.com/amangly/palepale-rs) as my agent harness.

I asked DeepSeek for a simple CS2 cheat. It added ESP, aimbot, triggerbot, and more, and the result was broken. That's why I built kiss. With the skill, the agent built only ESP, and it worked.

<table>
  <tr>
    <th width="50%">Before kiss</th>
    <th width="50%">With kiss: ESP only</th>
  </tr>
  <tr>
    <td width="50%" valign="top"><img src="assets/why-kiss.png" alt="The DeepSeek session that led me to build kiss" width="100%"></td>
    <td width="50%" valign="top"><img src="assets/esp-only-result.png" alt="ESP-only result after using kiss" width="100%"></td>
  </tr>
</table>

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
