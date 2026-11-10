# Wireframer

A Claude Code plugin that coaches a non-technical person from an app idea to a mapped screen flow, a clickable grey preview, and a brief for Claude Design. There are no commands to remember: they describe the idea and Claude suggests each next step.

The plugin is one skill, `plugins/wireframer/skills/app-wireframes/SKILL.md`.

## Test locally

From this folder:

```
claude plugin marketplace add ./
claude plugin install wireframer@wireframer
```

Then open Claude Code in an empty folder and describe an app idea. Pressing Shift+Tab once ("accept edits" mode) stops Claude asking before every file it writes.

After editing files here, run `claude plugin marketplace update wireframer`, then reinstall or restart Claude Code.

## Install from GitHub

Inside Claude Code:

```
/plugin marketplace add johnreitano/wireframer
/plugin install wireframer@wireframer
```

Then open Claude Code in a new folder for the app and describe the idea.
