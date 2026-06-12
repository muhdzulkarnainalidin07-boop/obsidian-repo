# Setup Guide

> Do this once. Takes about 10 minutes.

---

## Required plugins

Install these from Settings → Community Plugins → Browse:

| Plugin | Why you need it |
|---|---|
| **Dataview** | Powers all the automatic stats tables on the dashboard |
| **Templater** | Lets you create a new session note pre-filled with today's date |
| **QuickAdd** | Makes opening a new session a single keyboard shortcut |

All three are free and widely used — safe installs.

---

## Step 1 — Dataview setup

1. Install Dataview
2. Settings → Dataview → turn on **Enable JavaScript Queries** (needed for some calculations)
3. Leave everything else default

---

## Step 2 — Templater setup

1. Install Templater
2. Settings → Templater:
   - Set **Template folder location** to `Pool/Templates`
   - Turn on **Trigger Templater on new file creation**
3. Test: open command palette (`Ctrl+P` or `Cmd+P`) → "Templater: Create new note from template" → choose Session Template

---

## Step 3 — QuickAdd setup (fastest way to log)

1. Install QuickAdd
2. Settings → QuickAdd → Add choice → Name it `Pool: New Session` → Type: **Template**
3. Configure:
   - Template path: `Pool/Templates/Session Template.md`
   - File name format: `Pool/Sessions/{{DATE:YYYY-MM-DD}} Session`
   - Turn on **Open** (opens the note immediately after creation)
4. Back in QuickAdd settings → click the lightning bolt icon next to your macro to add it to the command palette
5. Settings → Hotkeys → search "QuickAdd: Pool: New Session" → assign `Ctrl+Shift+P` (or whatever feels natural)

After this, your session workflow is: one shortcut → note opens pre-filled → fill in your log before leaving the table.

---

## Step 4 — Folder structure check

Your vault should look like this:

```
Pool/
├── Dashboard.md          ← your home base
├── Sessions/             ← one note per session goes here
├── Reviews/              ← weekly review notes go here
├── Templates/
│   ├── Session Template.md
│   └── Weekly Review Template.md
└── Meta/
    ├── Drill Library.md
    └── Setup Guide.md    ← you're here
```

If you imported this as a zip, the structure is already set. Just move the whole `Pool/` folder into your main vault.

---

## Step 5 — Your first session note

1. Press your QuickAdd hotkey
2. The note opens with today's date already in the filename and frontmatter
3. Fill in: duration, session type, focus rating, tilt, one win, one next focus
4. Everything else is optional

That's a complete log. The dashboard will pick it up automatically.

---

## ADHD-specific tip

Pin the Dashboard note in your sidebar (right-click the tab → Pin). It's always one click away, and seeing the recent sessions table is a decent prompt to go practice.

## OCD-specific tip

The only fields that "count" are: `focus::` and `tilt::`. If those two are filled, the session is logged. Resist the urge to go back and fill in old sessions retroactively — forward only.

---

## Weekly review workflow

Once a week (Sunday works well, or day after your last session of the week):

1. Command palette → "Templater: Create new note from template" → Weekly Review Template
2. Save it to `Pool/Reviews/YYYY-WW Review.md`
3. The Dataview tables pull that week's sessions automatically
4. Takes 10–15 minutes

---

## Troubleshooting

**Tables show "No results"** — make sure your session notes are saved inside `Pool/Sessions/` exactly. Dataview queries path-match the folder name.

**Templater date isn't filling in** — make sure you're creating the note via Templater (not just duplicating a file). The `<% tp... %>` tags only execute through Templater.

**inline fields not showing in queries** — Dataview reads `fieldname:: value` syntax. Make sure there's no space before the `::` and the value is on the same line.
