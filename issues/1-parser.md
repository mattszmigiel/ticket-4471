Covers **379 reports** (of the 412 merged into #4471). 11 tenants, 2026-04-01 to 2026-10-04.

**Problem.** The shared parser reads every date month first. Day-first tenants get dates with day and month flipped (for example "Booked for 2 July, the invite says 7 February").

**Who.** harbour.dental, kettle.books, lantern.row, morrow.tax, long.table, ridge.clinic, alder.physio, pale.harbour, copper.studio, nine.lanterns, stone.and.sons. Reports come by app, email and (booking-v2) form.

**Notes.**
- This is the cause #4471 names. The queued fix belongs here.
- Intake tagged 23 of these `hint`. The tag is a guess; do not count by it.
- This count includes the 5 one-day reports in issue 3, as the desk's view files them. Three of the 379 carry no date to check (R-41290, R-41417, R-41514) and are placed by tenant only.
- Count is from the 2026-10-04 export; the live queue may be larger.
