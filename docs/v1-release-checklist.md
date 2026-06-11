# V1.0 Release Checklist

Use this checklist before calling the static demo ready for a public free release.

## Browser Demo

- Open `demo/index.html` with no console errors.
- Confirm the default vineyard, orchard, golf turf, and garden scenarios load with sensible managed areas.
- Generate a report from photo context, location, weather, map, sensor text, and optional notes.
- Save Low, Medium, and High records and confirm dashboard totals, risk trend, filters, search, sorting, and deletion.
- Confirm Markdown download, JSON history export, AI evidence packet download, weekly pilot Markdown, weekly pilot JSON, and browser Save as PDF workflow.
- Reset local demo data and confirm the default state restores cleanly.

## Location, Weather, And Map

- Use manual latitude and longitude and confirm report coordinates update.
- Use browser geolocation when available and confirm it updates inputs without overwriting managed area coordinates.
- Save current coordinates to a managed area and confirm they persist after refresh.
- Confirm the local map shows selected area, other areas, saved inspection points, and boundary sketches.
- Import weather from Open-Meteo when online and use sample weather fallback when offline.

## Evidence And Scouting Support

- Confirm local photo evidence extraction is labeled as role, filename, and notes based.
- Confirm Evidence Fusion Score explains source influence without claiming diagnosis.
- Confirm missing satellite NDVI shows `Unavailable` or `None`, not `Stable`.
- Import sample satellite NDVI and confirm trend labels can show Improving, Stable, Declining, or Unavailable.
- Confirm managed area boundaries are presented as scouting sketches, not surveyed GIS data.

## Pilot Readiness

- Fill the Pilot Mode intake form for vineyard, orchard, and golf course examples.
- Generate weekly reports after saving several records for a managed area.
- Check that expert review triggers and safety language appear for high-risk or uncertain cases.
- Confirm README, roadmap, backlog, pilot request form, and issue templates are linked and current.

## Release Notes

- The demo remains static and backend-free.
- Satellite, boundary, photo evidence, and fusion features are local demo support, not live satellite, hosted vision, precise GIS, or final diagnosis.
- V1.5 is the next planned step for hosted dashboard, accounts, scheduled refreshes, and team workflows.
