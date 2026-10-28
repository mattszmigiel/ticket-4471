Covers **33 reports** (of the 412 merged into #4471). 3 tenants, 2026-04-17 to 2026-09-22.

**Problem.** booking-v3 prints `MM/DD/YYYY` under the date field. Tenants that write day first type what the hint says (month first) and the form reads it their way, so the date is flipped. This is a form bug, not a parser bug; fixing the parser does not fix it.

**Who.** Form reports from alder.physio (12), copper.studio (11), pale.harbour (10), all on booking-v3.

**Notes.**
- Fix direction: the hint should follow the tenant's locale, or the form should read what its hint prints.
- Intake tagged 15 of these `parser`. The tag is a guess; do not count by it.
- Count is from the 2026-10-04 export; the live queue may be larger.
