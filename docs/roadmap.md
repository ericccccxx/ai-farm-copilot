# Roadmap

AI Farm Copilot should grow from a lightweight open-source agent skill into a practical decision layer for photos, sensors, drones, and farm equipment.

## V0: GitHub Launch

Goal: make the project understandable, installable, and easy to star.

- Agent skill package.
- README and positioning.
- Four scenario examples.
- Local browser demo.
- CSV data templates.
- Safety disclaimer.
- Hardware integration notes.

Success metric:

- Repository is ready to publish.
- A user can understand the project in less than 60 seconds.
- A user can run the demo without setup.
- A user can copy the skill into an agent environment.

## V0.1: Better Reports

- Add local image upload and preview.
- Add scenario-specific defaults.
- Add report severity scoring.
- Add follow-up task generation.
- Add exportable Markdown inspection report.

## V0.2: Saved Records

- Add multi-image preview.
- Add sensor and weather reading notes.
- Add local saved inspection records.
- Add saved record loading.
- Add JSON history export.

## V0.3: Managed Areas

- Add default managed areas.
- Add custom managed area creation.
- Attach saved inspection records to managed areas.
- Add area-level record count and latest risk summary.

## V0.4: Monitoring Dashboard

- Add global monitoring metrics.
- Add high-risk record count.
- Add area health cards.
- Add risk bars by managed area.
- Add latest inspection status by area.

## V0.5: Local Data Management

- Add saved record deletion.
- Add managed area update.
- Add managed area deletion.
- Add clear local demo data control.

## V0.6: Weather Import

- Add latitude and longitude inputs.
- Add Open-Meteo current weather import.
- Add sample weather fallback for offline demos.
- Write imported weather into report context and sensor notes.

## V0.7: Photo Intake

- Add photo role tagging.
- Add overview, affected, healthy comparison, close-up, drone, and sensor/equipment image roles.
- Add photo checklist to generated reports.
- Improve multi-photo comparison workflow.
- Add soil moisture CSV parser.
- Add irrigation schedule template.
- Add weekly field summary workflow.

## V0.8: CSV Import

- Add CSV file input.
- Parse sensor readings and inspection logs.
- Write latest CSV row into sensor notes.
- Add sample CSV for demos.

## V0.9: Camera and Drone Workflow

- Add batch photo naming convention.
- Add drone scouting checklist.
- Add camera mount guidance.
- Add image comparison workflow by date and block.
- Add filename parsing for date, area hints, and role detection.
- Add photo batch summary to reports.

## V0.10: Sensor Kit Support

- Add ESP32 JSON template.
- Add Raspberry Pi camera workflow.
- Add sensor calibration notes.
- Add low-cost field gateway architecture.
- Add JSON import for sensor gateway readings.
- Add pasted JSON and sample JSON workflows.

## V0.11: Vegetation Index

- Add NDVI calculation from NIR and Red values.
- Add vegetation vigor status.
- Add NDVI values to generated reports.

## V0.12: Advisor Mode

- Add advisor-style recommendation output.
- Add missing evidence summary.
- Add expert review triggers.
- Add 7-day care plan.
- Add compatibility notes for adjacent farm advisor skills.

## V0.13: Report Export

- Add browser print workflow.
- Add Save as PDF report export through the browser print dialog.
- Add print-specific report layout for cleaner field reports.

## V0.14: Agent Prompt Export

- Generate a copyable advisor prompt from the current inspection report.
- Add prompt download for Codex, Claude, and other agent workflows.
- Include safety boundaries, missing evidence, and requested output structure in the prompt.

## V0.15: Scenario Prompt Templates

- Add vineyard, orchard, golf turf, and home garden prompt presets.
- Tune each prompt with scenario-specific focus areas and missing evidence requests.
- Show the active advisor template in the report interface.

## V0.16: History Trend

- Add a saved inspection risk trend chart.
- Show recent risk movement from local history.
- Keep the chart browser-only and compatible with GitHub Pages.

## V0.17: Dashboard Scope Filters

- Add dashboard scope filtering for all areas, current selected area, and specific managed areas.
- Update dashboard metrics, risk trend, and area health cards based on the selected scope.
- Keep filtering local and browser-only.

## V0.18: Dashboard Risk Filters

- Add high, medium, and low-risk filters to the monitoring dashboard.
- Apply risk filtering to dashboard metrics, risk trend, and area health cards.
- Show a clear empty state when no saved records match the active filters.

## V0.19: Saved Record Search

- Add saved record search.
- Match records by crop, area, scenario, risk, notes, weather, sensor data, and report text.
- Show a clear empty state when no records match the search.

## V0.20: Saved Record Sorting

- Add saved record sorting controls.
- Sort saved records by newest, oldest, highest risk, and lowest risk.
- Keep sorting compatible with saved record search.

## V0.21: Saved Record Quick Filters

- Add quick filters for all saved records, high-risk records, current area, and recent 7 days.
- Keep quick filters compatible with saved record sorting.
- Make manual search return to normal search behavior.

## V0.22: Per-Area Trend Lines

- Add mini risk trend lines to area health cards.
- Show recent risk movement for each managed area.
- Keep the trend display lightweight and browser-only.

## V0.23: Area Detail View

- Add a selected-area detail panel.
- Show latest inspection date, highest saved risk, next action, and recent history.
- Refresh area detail when records or selected area change.

## V0.24: Date Range Filters

- Add dashboard date range filtering for all dates, last 7 days, and last 30 days.
- Add saved record date range filtering for all dates, last 7 days, and last 30 days.
- Keep date filters compatible with search, sorting, quick filters, area filters, and risk filters.

## V0.25: Automatic Location

- Add a Use My Location control. Done in V0.25.
- Use browser geolocation to fill latitude and longitude after user permission. Done in V0.25.
- Keep manual latitude and longitude input as the fallback. Done in V0.25.
- Show clear success, denied, timeout, and unsupported states. Done in V0.25.

## V0.26: Local Time and Timezone

- Read browser timezone with `Intl.DateTimeFormat().resolvedOptions().timeZone`. Done in V0.26.
- Add local inspection time, timezone, and timestamp to reports and saved records. Done in V0.26.
- Use local time formatting in saved records and reports. Done in V0.26.
- Pass timezone into weather requests where supported. Done in V0.26.

## V0.27: Weather Forecast Risk

- Extend Open-Meteo import from current weather to 7-day forecast. Done in V0.27.
- Add weather risk notes for heat, wind, high humidity, no rain, and post-rain disease pressure. Done in V0.27.
- Add forecast risk warnings to the report context and sensor notes. Done in V0.27.

## V0.28: Map Location View

- Add a map panel centered on the current GPS coordinates. Done in V0.28.
- Show managed areas and saved inspection points on the map. Done in V0.28.
- Store center coordinates for managed areas. Done in V0.28.

## V0.29: Managed Area Boundaries

- Add simple boundary drawing for vineyard blocks, orchard zones, golf zones, and garden beds. Done in V0.29.
- Store polygon boundaries locally. Done in V0.29.
- Attach saved inspections to area boundaries for later satellite clipping. Done in V0.29.

## V0.30: Satellite Basemap MVP

- Add a satellite-style map layer. Done in V0.30.
- Show current location, managed areas, and saved inspection points over the basemap. Done in V0.30.
- Prioritize visual clarity before advanced agronomic analysis. Done in V0.30.

## V0.31: Satellite NDVI Data

- Connect a satellite data source for NDVI when an area boundary is available. Done in V0.31.
- Add cloud-aware recent image selection. Done in V0.31.
- Add satellite vegetation notes to the report. Done in V0.31.

## V0.32: Satellite Time Comparison

- Compare current and previous NDVI readings. Done in V0.32.
- Classify satellite trend as improving, stable, declining, or unavailable. Done in V0.32.
- Add NDVI trend to dashboard and area detail. Done in V0.32.

## V0.33: Photo AI Evidence

- Add optional vision-model analysis for uploaded photos. Done in V0.33.
- Extract visible symptoms, affected plant parts, image quality, and missing photo requests. Done in V0.33.
- Treat photo AI output as evidence, not a final diagnosis. Done in V0.33.

## V0.34: Evidence Fusion Score

- Combine photo, weather, satellite, history, and sensor signals into a risk score. Done in V0.34.
- Show which evidence sources influenced the risk decision. Done in V0.34.
- Keep recommendations cautious and evidence-based. Done in V0.34.

## V0.35: One-Click AI Report

- Let users generate a full inspection report from photo, location, and scenario with minimal manual input. Done in V0.35.
- Make manual notes optional context instead of required context. Done in V0.35.
- Produce an AI-ready evidence packet for Codex, Claude, or GPT. Done in V0.35.

## V0.36: Pilot Mode

- Add pilot customer workflow for vineyards, orchards, and golf courses.
- Export weekly reports in Markdown, JSON, and browser PDF.
- Add pilot intake form and reporting checklist.

## V1.0: Free Usable Release

- GitHub Pages demo, agent skill, and documentation are complete.
- Photo, location, weather, map, history, and report flow can run end to end.
- Satellite and vision AI remain optional integrations.
- README clearly explains open-source use, agent use, hardware use, and drone/robot compatibility.

## V1.5: Hosted Dashboard

- Add accounts, cloud-saved areas, and cloud-saved inspections.
- Add team access.
- Run scheduled weather and satellite refreshes.
- Add email or SMS alerts for high-risk areas.

## V2.0: Hardware Decision Layer

- Support camera, drone, Raspberry Pi, ESP32, and robot data uploads.
- Accept photos, sensor JSON, location, weather, and satellite data.
- Output risk, tasks, routes, recheck timing, and reports for people or equipment.
