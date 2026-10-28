Covers **5 reports** (of the 412 merged into #4471). 5 tenants, 2026-04-02 to 2026-10-04.

**Problem.** The date is off by one day. Day and month are intact, so this is not a month/day swap. Examples: "Tuesday 12 May" shows as "Monday 11 May"; one meeting is Tuesday for a client in Lisbon and Monday for a client in Toronto; an invite arrives before the booking was made.

**Reports.** R-41202 (kettle.books), R-41209 (alder.physio), R-41236 (nine.lanterns), R-41344 (pale.harbour), R-41620 (lantern.row).

**Suspect.** A timezone or DST problem. This is a reading of the report text, not confirmed.

**Notes.**
- The desk notes list these as `oneDayMove`. The old table counted them under `parser`.
- All five were tagged `parser` by intake.
- Count is from the 2026-10-04 export; the live queue may be larger.
