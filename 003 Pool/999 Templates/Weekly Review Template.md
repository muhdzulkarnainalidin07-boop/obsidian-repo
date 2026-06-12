---
week: <% tp.date.now("YYYY-[W]WW") %>
date_start: <% tp.date.now("YYYY-MM-DD", -tp.date.now("d") + 1) %>
date_end: <% tp.date.now("YYYY-MM-DD", 7 - tp.date.now("d")) %>
tags: [pool, weekly-review]
---

# Week <% tp.date.now("[W]WW") %> — Pool Review

## Sessions this week

```dataview
TABLE duration + " min" AS Duration, session_type AS Type, focus AS Focus, tilt AS Tilt
FROM "003 Pool/Sessions"
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
FROM "Pool/Sessions"
WHERE date >= this.date_start AND date <= this.date_end
SORT date ASC
```

---

## Next week's priority

> One mechanical thing and one mental thing.

**Mechanical:**

**Mental:**

---

## Honesty check

- [ ] Did I actually practice what I said I would last week?
- [ ] Am I repeating the same drills without making them harder?
- [ ] Am I logging honestly, or rounding up my ratings?
