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

## V1: Commercial-Ready Layer

- Hosted dashboard.
- Team accounts.
- Saved fields, blocks, and reports.
- Hardware kit partnerships.
- Vineyard, orchard, and golf turf pilot programs.
