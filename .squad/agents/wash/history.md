## Learnings

### 2026-06-04 — Project kickoff
- Project: EV Charging Station Simulator
- Requested by: Lyle MS Luppes
- My domain: game loop, vehicle state machine, charging math, FIFO queue
- FR-007 formula: durationSeconds = clamp(((targetPct - startPct) / 100 * capacityKWh) / powerKw * 3600, 30, 90)
- Queue behavior: FIFO, cars wait visually when bays full, dequeue when bay opens
- Reset must be atomic — one tick, no orphaned state
- Idempotent clicks: ignore re-clicks on non-roadway vehicles
