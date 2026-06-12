---
week: 2026-W24
date_start: 2026-06-08
date_end: 2026-06-14
tags: [pool, weekly-review]
---

# Week W24 — Pool Review

## Sessions this week

```dataview
TABLE duration + " min" AS Duration, session_type AS Type, focus AS Focus, tilt AS Tilt
FROM "003 Pool/01 Sessions"
WHERE date >= this.date_start AND date <= this.date_end
SORT date ASC
```

---

## What I actually worked on

> Look back at your drill tables. What themes came up?



---

## Patterns I noticed

> Mechanical, mental, or positional — anything recurring.



---

## Focus rating trend

```dataview
TABLE date, focus AS "Focus (1–5)", tilt AS Tilt, win AS "What clicked"
FROM "003 Pool/01 Sessions"
WHERE date >= this.date_start AND date <= this.date_end
SORT date ASC
```

---

## Next week's priority

> One mechanical thing and one mental thing.

**Mechanical:** Speed Control

**Mental:** focus

---

## Honesty check

- [ ] Did I actually practice what I said I would last week?
- [ ] Am I repeating the same drills without making them harder?
- [x] Am I logging honestly, or rounding up my ratings?
