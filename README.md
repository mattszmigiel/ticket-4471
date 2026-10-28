# ticket-4471

Support desk ticket #4471 merged 412 date reports into one issue. Read by tenant, channel and report text, they are two problems. Each has its own issue here. Five of the parser reports read as a one-day move; the desk files them under parser, and the parser issue notes them.

| Issue | Cause | Reports |
|---|---|---|
| parser | shared parser reads dates month first | 379 (includes the 5 below) |
| hint | booking-v3 hint says MM/DD/YYYY to day-first tenants | 33 |

379 + 33 = 412 unique reports (the export had 427 rows; 15 repeat an id). Counted from the 2026-10-04 kb export.

- Page: `src/routes/kb/incidents/4471-three-causes/+page.svx` (signed, desk ref DR-7KF0-4GQY)
- Page as the desk sees it: `rendered/4471-three-causes.html`
