# Repository Context for AI Agents

Read this file before making any changes to this repository. It is the single source of truth for structure, conventions, and current academic status.

---

## What This Repository Is

An academic portfolio for Samuel Stidham's Computer Science education at Southern New Hampshire University (SNHU). It tracks coursework, grades, and reflections across the Bachelor of Science and the planned Master of Science in Computer Science.

**Academic integrity note:** This is a public portfolio. Specific assignment solutions, code submissions, or graded work are never included, in keeping with SNHU's academic integrity policy. Do not add them.

---

## Repository Structure

```
README.md          ← Landing page / index. Links to both degree program pages.
bachelors.md       ← Full BS program: course list, grades, and schedule.
masters.md         ← MS program placeholder (to be populated starting ~2028).
docs/
  2025/            ← Year 1 completed courses
  2026/            ← Year 2 courses (completed, in-progress, and planned)
  2027/            ← Year 3 courses (all planned, per advisor schedule)
  course-template.md           ← Template for completed courses
  upcoming-course-template.md  ← Template for planned/in-progress courses
.agents/
  core.md          ← This file
```

---

## File Naming Convention

Course files follow a strict sequential numbering scheme reflecting chronological order:

```
docs/<year>/<##> - <COURSECODE>.md
```

Example: `docs/2026/08 - CS210.md`

- Numbers start at `01` and increment by 1 for each course taken
- Numbers are never reused or skipped
- The next available number is **29**
- The year folder reflects the calendar year the course is taken, not the academic year

---

## Status System (used in bachelors.md and course lists)

| Symbol | Meaning |
| --- | --- |
| ✅ | Completed — final grade received |
| ⏳ | Upcoming or In Progress |

Back links in all course files use:
```
[← Back to Central Portfolio](../../bachelors.md)
```

---

## Current Degree Status (as of June 2026)

| Field | Value |
| --- | --- |
| Program | Bachelor of Science in Computer Science |
| Concentration | None (dropped to maximize transfer credit application) |
| Minor | Mathematics |
| Overall GPA | 4.000 |
| Credits Applied | 75 / 120 (includes completed, in-progress, and pre-registered) |
| Credits Remaining | 45 |
| Projected Graduation | December 2027 |

---

## Advisor-Confirmed Course Schedule

| Term | Dates | Courses |
| --- | --- | --- |
| 2026 C-3 | May–Jun 2026 | CS-210, PHY-150 *(In Progress)* |
| 2026 C-4 | Jun–Aug 2026 | MAT-230, CS-250 |
| 2026 C-5 | Aug–Oct 2026 | CS-300, DAD-220 |
| 2026 C-6 | Oct–Dec 2026 | CS-230, CS-305, MAT-350 |
| 2027 C-1 | Jan–Feb 2027 | CS-255, MAT-299 |
| 2027 C-2 | Mar–Apr 2027 | CS-320, MAT-415 |
| 2027 C-3 | May–Jun 2027 | CS-330, IDS-410 |
| 2027 C-4 | Jun–Aug 2027 | CS-340, MAT-243 |
| 2027 C-5 | Aug–Oct 2027 | CS-465, CS-360 |
| 2027 C-6 | Oct–Dec 2027 | CS-499, CS-370 |

CS-320 → CS-340 → CS-465 → CS-499 are locked prerequisite chains. Do not reorder them.

---

## Course File Formats

### Upcoming / In-Progress courses (`upcoming-course-template.md`)

```markdown
# <DESIGNATION> <COURSE NAME>

## Course Summary

| Category | Value |
| :--- | :--- |
| **Designation** | <e.g. CS-210> |
| **Name** | <Full course name> |
| **Planned Term** | <e.g. 2026 C-3 (May – Jun)> |
| **Status** | Upcoming |

**Course Description:**
<Official SNHU catalog description — one paragraph, no edits.>

---

[← Back to Central Portfolio](../../bachelors.md)
```

### Completed courses (`course-template.md`)

Same header as above, plus:
- `**Term Taken**` and `**Final Grade**` replace `**Planned Term**` and `**Status**`
- `## Key Topics & Concepts` section
- `## Major Projects & Assignments` section (no actual solutions)
- `## Personal Reflection & Takeaways` section
- `## External Resources` section

---

## How to Update This Repository

| Event | Action |
| --- | --- |
| Course starts | Update status to "In Progress" in `bachelors.md` table |
| Course completes | Convert file to completed template; add final grade to `bachelors.md`; change ⏳ to ✅ |
| New course registered | Create file with `upcoming-course-template.md`; assign next sequential number; add row to `bachelors.md` table and course lists |
| Degree status changes | Update the "Current Degree Status" table in this file AND in `bachelors.md` |
| MS program begins | Populate `masters.md` following the same structure as `bachelors.md`; add `docs/2028/` (or relevant year) |
