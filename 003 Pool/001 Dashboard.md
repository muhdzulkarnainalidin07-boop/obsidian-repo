# Pool Dashboard

> Your single entry point. All stats pull automatically from session notes.

---

## Start a session

> Use Templater: `Alt+N` → Session Template
> Or QuickAdd: `Ctrl+Shift+P` → Pool: New Session

---

## Recent sessions

```dataview
TABLE date AS Date, duration + " min" AS Duration, session_type AS Type, focus AS "Focus", tilt AS Tilt, win AS "What clicked"
FROM "003 Pool/01 Sessions"
SORT date DESC
LIMIT 10
```

---

## Focus trend (last 20 sessions)

```dataview
TABLE date AS Date, focus AS "Focus (1–5)", tilt AS Tilt, psr_consistent AS PSR, decision_quality AS "Decisions"
FROM "003 Pool/01 Sessions"
SORT date DESC
LIMIT 20
```

---

## Runout rate

```dataview
TABLE date AS Date, runouts_attempted AS Att, runouts_made AS Made
FROM "003 Pool/01 Sessions"
WHERE runouts_attempted != null AND runouts_attempted != ""
SORT date DESC
LIMIT 15
```

---

## What's been clicking (wins log)

```dataview
TABLE date AS Date, win AS "What clicked", next_focus AS "Planned next"
FROM "003 Pool/01 Sessions"
WHERE win != null AND win != ""
SORT date DESC
LIMIT 15
```

---

## Tilt events log

```dataview
TABLE date AS Date, tilt AS Tilt, focus AS Focus, duration + " min" AS Duration
FROM "003 Pool/01 Sessions"
WHERE tilt != "none" AND tilt != null AND tilt != ""
SORT date DESC
```

> Use this to find patterns — time of day, session length, certain drills?

---

## Weekly reviews

```dataview
TABLE week AS Week, file.link AS Review
FROM "003 Pool/02 Reviews"
SORT week DESC
LIMIT 8
```

---

## Drill reference

[[Drill Library]]

---

## Meta

- [[Setup Guide]] — Templater, QuickAdd, Dataview config
- Folder: `Pool/Sessions/` — all session notes live here
- Folder: `Pool/Reviews/` — weekly reviews live here
