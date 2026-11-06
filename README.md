# Deepkoi

A focus tracker for the Mac. Start a session on one task in a click, come
back to it after every break or distraction, and see where your time
really goes. Everything stays on your Mac: no account, and Deepkoi
connects only when you click **Check for Updates**.

Needs macOS 26 or later on a Mac with Apple silicon.

**[Download the latest version](https://github.com/aslandev2k/deepkoi-home/releases/latest)**

## Features

### Focus sessions
- Start a session on a task from the sticky bar, the menu bar, the
  start-session popup (Option-Space, changeable), or the dashboard.
- Take a break or report an interruption with a reason, then resume in one
  click.
- At time's up, extend the session or end it, from the sticky bar or the
  notification.
- End a session with a note on what you got done, and mark the task done
  at the same time.
- The sticky bar always shows what you are working on. Double-click it to
  open the task in focus.
- Full screen focus mode.
- Sessions pause on their own when you step away, and a reminder tells you
  when a break runs long.
- Background music while you focus, from mp3 files you add in Settings.

### Epics and tasks
- Group tasks into epics, each with its own color and icon.
- Create, edit, move, finish, reopen, and delete tasks, with rich text
  notes.

### Where your time goes
- Dashboard: today's focus, the streak, what distracted you, and your last
  7 days.
- Time log: every session of a week, day by day. Fix a reason, move a
  session to another task, or delete it.
- Report: real focus, focus rate, hours by epic, and top reasons for a
  week, a month, or a year, filtered by epic.

### On your Mac
- Menu bar item with the time left and a quick dropdown.
- Launch at login. The app and the sticky bar keep running when the main
  window closes.
- Settings for the accent color, focus, the sticky bar, epics, music,
  sounds, and optional features.
- Everything stays in `~/Library/Application Support/Deepkoi/`.
- Deepkoi > Check for Updates (Option-Command-U) finds a newer version,
  shows what is new, and installs it. Your data is backed up first.

## Install

1. Download `Deepkoi-<version>.dmg` from the
   [latest release](https://github.com/aslandev2k/deepkoi-home/releases/latest).
2. Open it and drag **Deepkoi** onto **Applications**.
3. Open Deepkoi from Applications. The first time, macOS stops it with a
   message that it could not check the app, because Deepkoi is not
   notarized by Apple. Click **Done** (not Move to Trash).
4. Open **System Settings > Privacy & Security**, scroll down to the
   message about Deepkoi, and click **Open Anyway**. Confirm with your
   password or Touch ID, then click **Open**.

You only do this once. After that Deepkoi opens like any other app.
Each new version you download asks once again.

If you prefer, `Deepkoi-<version>.zip` holds the same app. To check a
download, compare it with `SHA256SUMS.txt` in the release:

```sh
shasum -a 256 -c SHA256SUMS.txt
```

## Versions

See [Releases](https://github.com/aslandev2k/deepkoi-home/releases) for
what each version brought. Version 1.0.0 has no Check for Updates, so start
from the latest version.

## This repository

This repository serves Deepkoi's downloads and its update feed:

- `appcast.xml` is the feed that Deepkoi > Check for Updates reads, at
  https://aslandev2k.github.io/deepkoi-home/appcast.xml. Each entry is
  signed with Deepkoi's own update key.
- `notes/<version>.html` are the release notes shown before an update.
- Each release holds the disk image, a zip of the same app, and
  `SHA256SUMS.txt`.
