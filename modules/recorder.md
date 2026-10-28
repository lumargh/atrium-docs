---
title: Recorder
parent: Modules
nav_order: 7
---

# Recorder

The Recorder module records from your microphone into today's daily note. Its three buttons, also on its right-click menu, behind its ⋯ and as commands, are:

- **Record** (r): saves the sound as an attachment named like Obsidian's own recordings (`Recording 20261025142000.webm`) and adds it to the daily note on a timed line, `- [2:20 PM - 2:22 PM] ![[Recording 20261025142000.webm]]`, so it shows on the agenda too.
- **Dictate** (d), on macOS 26 and later: what you say shows in the card as you speak, the words that may still change dimmed, and stopping adds it to the daily note as one timed line, `- [2:20 PM - 2:22 PM] Buy milk and call the dentist at 9.` It's transcribed on your Mac by Apple's speech recognition, in your system language; the first time, macOS downloads that language's model. **Keep audio with dictation**, in the card's settings, saves the recording too, on a line under the text.
- **Speak a command** (c), on macOS 26 and later: listens until you pause. First it tries a few phrases that name what they act on:
  - "open the agenda", "add timer", "show music": picks out that card, unfolding it or bringing it forward in its stack, or adds it if the page has none.
  - "go to tomorrow", "Friday", "next Tuesday", "last Monday", "October 30th": shows that day.
  - "switch to Work", "open Home workspace": opens that workspace.

  Otherwise it runs the command whose name has every word you said, such as "fold music" or "next workspace", on the card you name or else the one picked out before. Words like "the" and "card" are left out, a word can match by its start, and some count as one: open, show, view and display; add, new, create and insert; next and forward; previous and back; fold and collapse. Failing that, "open" and a note's name, such as "open meeting notes", opens that note in a new tab, if one note has that name or starts with it. If nothing matches, a command picker opens with your words, to pick from or change.
- **Ask Claude Code**: with [Claude Code](https://claude.com/claude-code) installed, this setting in the card's settings sends what no command matches to Claude Code instead of the picker. It brings your Terminal card forward, or adds one, and runs `claude` with your words there, so you can follow and answer it.

**History**, folded under the buttons once you've spoken a command, lists the latest twenty, newest first. A click runs one again; its right-click menu has **Run again** and **Remove from history**.

While it's under way, a visualizer moves with your voice and the button turns to **Stop and save**; the key that started it stops it too.
