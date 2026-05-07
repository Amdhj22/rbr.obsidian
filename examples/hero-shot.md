---
created: 2026-05-07 11:50
tags: [theme, hero, demo, rbr]
---

# RBR — Three-accent navy theme

> Kerb red marks the **active**. RB yellow flags **attention**. Chequer white points to **functions**. Everything else steps back.

## Trio at a glance #theme #obsidian #f1

The trio drives every choice — **bold takes white**, *italic carries livery blue*, and ==yellow highlights== call you back. ~~Strikethrough~~ fades into subtext.

### Diagnostics callouts

> [!warning] Warning
> RB Yellow flags what needs attention before the next lap.

> [!tip] Tip
> Paddock green carries success — added files, passing tests.

> [!error] Error
> Kerb **bright** owns errors and deletions. Kerb **red** is reserved for "this one."

> [!info] Info
> Oracle blue handles info, links, and the k8s context indicator.

### Code — syntax trio

```rust
use std::collections::HashMap;

/// Sector delta against the pole lap.
/// Returns total time gained or lost across all sectors.
pub fn lap_delta(reference: &Lap, current: &Lap) -> f64 {
    let mut total = 0.0_f64;
    for (sector, time) in current.sectors.iter().enumerate() {
        total += time - reference.sectors[sector];
    }
    total
}

const PIT_LIMITER: f32 = 80.0;
const DRS_ZONES: usize = 3;
```

Inline call: `lap_delta(&pole, &current)` — `lap_delta` lights up **chequer white** as the third accent at every call site.

### Standings

| # | Driver | Team | Best lap | Δ leader |
|---:|---|---|---:|---:|
| 1 | Verstappen | Red Bull | 1:18.234 | — |
| 2 | Pérez | Red Bull | 1:18.501 | +0.267 |
| 3 | Leclerc | Ferrari | 1:18.647 | +0.413 |

### Lap notes

1. Set up the corner
2. Trail-brake to the apex
3. Power down on exit

- [x] Brake earlier into Turn 7
- [ ] Carry more apex speed
- [ ] Trail throttle on exit

> "If you no longer go for a gap that exists, you are no longer a racing driver." — Ayrton Senna

#### h4 — paddock green

##### h5 — oracle blue

###### h6 — sky blue

---

[Style Settings plugin](https://github.com/mgmeyers/obsidian-style-settings) · [[Architecture]] · [[NotAFile]]
