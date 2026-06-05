## Learnings

### 2026-06-04 — Project kickoff
- Project: EV Charging Station Simulator
- Requested by: Lyle MS Luppes
- My role: rubber duck reviewer and QA
- Key risks to watch: orphaned vehicle state on reset, FIFO queue not draining on bay free, idempotent click handling, queue visual ordering
- AC-011 (300ms debounce), AC-012 (atomic reset), AC-006 (full-capacity behavior) are highest-risk acceptance criteria
