# Shamsi Calendar data

Iran's official lunar (Hijri) month starts, read by the Shamsi Calendar app.
The app ships with a copy of this file and checks this repository about once
a week, so a new year's dates reach every install without an app update.

## Format

`hijri-months.json`:

```json
{
  "version": 1,
  "months": [[1448, 6, "2026-11-11"], ...]
}
```

Each entry is `[hijriYear, hijriMonth (1-12), first day of the month (Gregorian, YYYY-MM-DD)]`.
The app ignores the whole file if any entry is malformed. A month the file
lists overrides the app's built-in copy of that month.

## Yearly update

When the Calendar Center of the University of Tehran's Institute of
Geophysics publishes the next official calendar, add its twelve month starts
here. If a month is announced differently after moon sighting, correct its
start date.

## Sources

- https://github.com/roozbehp/qamari (CC0-1.0): official month starts from
  1400 AH onward.
- Official calendar 1405, Calendar Center, Institute of Geophysics, University
  of Tehran: month starts from Dhu al-Qa'dah 1447 to Shawwal 1448.

## License

CC0 1.0 Universal (public domain), like the qamari data it builds on.
