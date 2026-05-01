# THCC Scheduler

A self-contained HTML scheduling utility for Tree House Cannabis Co. dispensary locations.

## Features

- **Weekly Schedule Grid** — interactive shift assignment with role grouping (GM → Keyholders → Associates)
- **Gantt View** — daily horizontal bar chart showing all shifts on a 7am–midnight time axis
- **Staff & Availability** — full staff directory with days-off survey data from Airtable
- **Availability Update Form** — update any staff member's days off and notes in-tool
- **Conflicts Tab** — auto-detects availability violations, medical hour caps, and missing MOD coverage
- **Hours Summary** — per-staff scheduled hours vs. prior week baseline
- **Import / Export** — generates Shifts-compatible CSV for direct import; full JSON round-trip save/restore

## Shift Types

| Type | Label | Times |
|------|-------|-------|
| `open` | MOD Open | 7:00 AM – 3:30 PM |
| `open-security` | Security Open | 7:30 AM – 3:30 PM |
| `open-greeter` | Greeter Open | 7:30 AM – 3:30 PM |
| `mid` | MOD Mid | 11:30 AM – 8:00 PM |
| `mid-bt` | Mid | 12:00 PM – 8:00 PM |
| `close-wed` | MOD Close | 2:00 PM – 10:30 PM (Sun–Wed) |
| `close-thu` | MOD Close | 3:00 PM – 11:00 PM (Thu–Sat) |
| `close-wed-security` | Security Close | 2:30 PM – 10:00 PM (Sun–Wed) |
| `close-thu-security` | Security Close | 2:30 PM – 11:00 PM (Thu–Sat) |
| `close-wed-greeter` | Greeter Close | 2:30 PM – 10:00 PM (Sun–Wed) |
| `close-thu-greeter` | Greeter Close | 2:30 PM – 11:00 PM (Thu–Sat) |
| `close-late-sw` | Cashier Close | 3:00 PM – 11:30 PM (Sun–Wed) |
| `close-late-th` | Cashier Close | 3:30 PM – 11:30 PM (Thu–Sat) |

## Store Hours

| Days | Open | Close |
|------|------|-------|
| Sunday – Wednesday | 8:00 AM | 10:00 PM |
| Thursday – Saturday | 8:00 AM | 11:00 PM |

## Usage

Open `dracut_scheduler.html` directly in any modern browser — no server or dependencies required.

To load a saved schedule, use the **Import / Export** tab and paste in a previously exported JSON.

## Location

Currently configured for the **Dracut** location with the extended hours model (effective Q2 2026).
