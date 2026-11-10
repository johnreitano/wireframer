---
name: app-wireframes
description: Use when someone wants wireframes, mock-ups, screens or a prototype for an app or website idea, or wants to continue working on one. Adds a few habits to keep the screen flow sound and ready for Claude Design.
---

# App wireframes

Help as you normally would. The person is probably not technical, so use plain words, do the work yourself, and end each reply with the one next step you suggest. Follow these extra habits.

## Keep a written screen list

Keep `flow.md` in the project folder as the record of the app: every screen, what's on it, and where each button goes, plus a Mermaid diagram of how screens connect. Change `flow.md` first whenever the flow changes, then update anything built from it. When someone comes back to the project, read `flow.md` and recap in one line where things stand.

## Check before showing

Before you show a set of screens, check them for:
- dead ends (a screen with no way onward or back) and taps that go nowhere
- screens nothing leads to
- sign-up, sign-in and forgot password, if there are accounts
- empty lists, errors (wrong password, card declined, no internet) and confirmations
- "are you sure?" before cancelling or deleting

Fix the gaps and say in plain words what you added.

## Pause for review

Show the screen list and ask for changes before building anything clickable, and ask again before the Claude Design hand-off. "Yes" or "what's next?" means carry on to the step you suggested.

## Write the clickable screens directly

Build them in a `preview/` folder: one plain HTML file per screen, linked with ordinary links, one shared `style.css`, and an `index.html` listing every screen. Avoid single-page apps that show and hide screens with JavaScript, because when they break every screen piles on top of the others. Write the files with your file tools; don't write or run scripts to generate them, because the permission prompt confuses non-technical people. After building, check that every link points at a file that exists.

Keep the preview grey. Don't add colours or styling yourself; the look comes from Claude Design.

## Hand off to Claude Design

When the preview's flow is settled, write `design-brief.md` for Claude Design (in the Claude app): a short summary of the app, the placeholder brand (name, colours, font, feel), and each screen in order with what's on it and where its buttons go. Split it into parts if there are more than about 15 screens. Then tell them in a few steps how to paste it into Claude Design.

## Suggest testing with real people

Once there's a clickable version, suggest showing it to three or four likely users with one task each, and bringing back where they got stuck.
