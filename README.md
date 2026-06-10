# AI Farm Copilot

Open-source AI farm and garden copilot for vineyards, orchards, golf turf, hobby farms, and home gardens.

AI Farm Copilot is a lightweight, agent-native toolkit that helps growers, groundskeepers, and land owners turn field observations into practical inspection notes and care plans. It is designed to work with Codex, Claude, and other AI agents through a reusable skill package.

> Core promise: take a plant or turf photo, add a few field conditions, and get a structured inspection report with risk level, likely causes, recommended actions, and next check-in timing.

## Who This Is For

- Vineyard operators who need fast scouting notes before problems spread.
- Orchard managers who want a simple way to log tree health, irrigation concerns, and pest pressure.
- Golf course superintendents and turf teams who need quick visual triage for stressed areas.
- Hobby farm and home garden owners who want an AI assistant without expensive farm software.
- Hardware builders who want an open decision layer for cameras, drones, sensors, robots, or small tractors.

## What It Does

- Guides an AI agent through crop, turf, and garden inspection workflows.
- Uses photos plus user-provided context such as weather, irrigation, soil, and recent treatments.
- Produces structured reports: observations, possible causes, risk level, suggested actions, and follow-up plan.
- Includes starter scenarios for vineyards, orchards, golf turf, and home gardens.
- Provides CSV templates for field logs, weather data, soil readings, and sensor readings.
- Offers a simple browser demo to show the user experience before deeper integrations.

## What This Is Not

AI Farm Copilot is not a replacement for a certified agronomist, pesticide adviser, turf expert, irrigation engineer, or local compliance authority. The project helps organize observations and suggest next checks. High-risk decisions, chemical applications, disease confirmation, and major irrigation changes should be reviewed by qualified professionals.

## Quick Start

### Use the AI Skill

1. Copy `skills/ai-farm-copilot` into your Codex or Claude skills directory.
2. Start a new agent session.
3. Ask: `Use the AI Farm Copilot skill to inspect my vineyard block from this photo and field notes.`
4. Provide a photo and basic context when the agent asks.

### Try the Demo

Open `demo/index.html` in your browser. The demo runs locally and does not send data anywhere.

The V0.32 demo supports:

- Local multi-image upload and preview.
- Local map location view for current coordinates, managed areas, and saved inspection points.
- Satellite-style local basemap layer with a field sketch fallback.
- Local satellite NDVI adapter with cloud-aware recent image selection when an area boundary is available.
- Satellite NDVI trend comparison against a previous selected image.
- NDVI trend status in the monitoring dashboard and selected-area detail view.
- Satellite vegetation notes written into reports and Advisor Mode.
- Managed area center coordinates with a manual "Use Current Coordinates for Area" save control.
- Risk-colored saved inspection markers on the local map.
- Managed area boundary sketches with saved polygon points.
- Boundary snapshots attached to saved inspection records for later satellite clipping workflows.
- Photo role tagging for overview, affected area, healthy comparison, close-up, drone, and sensor/equipment images.
- Batch photo filename parsing for date, area hints, and role detection.
- Drone/camera batch summary in generated reports.
- Photo checklist output in inspection reports.
- CSV import for sensor readings or inspection logs.
- Sample CSV import for demos.
- JSON import for ESP32, Raspberry Pi, camera node, or sensor gateway readings.
- Pasted JSON and sample JSON workflows.
- NDVI calculation from NIR and Red values.
- Vegetation vigor status in Sensor Notes.
- Advisor Mode with missing evidence, decision posture, expert review triggers, and a 7-day care plan.
- Copyable and downloadable agent prompt for Codex, Claude, or other advisor workflows.
- Scenario-specific agent prompt templates for vineyard, orchard, golf turf, and home garden workflows.
- Managed area records for vineyard blocks, orchard sections, golf zones, and garden beds.
- Managed area update and delete controls.
- Monitoring dashboard with area counts, record counts, high-risk count, and latest risk.
- Risk trend chart from saved inspection history.
- Dashboard scope filtering for all areas, the current selected area, or one managed area.
- Dashboard risk filtering for high, medium, and low-risk saved records.
- Dashboard date range filtering for all dates, last 7 days, and last 30 days.
- Area health cards with risk bars and recent inspection status.
- Per-area mini trend lines in area health cards.
- Area detail view with latest inspection, highest risk, next action, and recent history.
- Open-Meteo weather import using latitude and longitude.
- Browser geolocation with Use My Location and manual coordinate fallback.
- Local timezone and local inspection time in reports and saved records.
- 7-day weather forecast risk notes for heat, dry conditions, wind, humidity, and post-rain disease pressure.
- Sample weather fallback for offline demos.
- Scenario-specific defaults for vineyard, orchard, golf turf, and home garden.
- Sensor and weather reading notes.
- Dynamic risk level and follow-up timing.
- Structured report generation.
- Markdown report download.
- Browser print and Save as PDF report export.
- Local saved inspection records.
- Saved record search across crop, area, risk, notes, weather, and sensor text.
- Saved record sorting by newest, oldest, highest risk, and lowest risk.
- Saved record quick filters for all records, high risk, current area, and recent 7 days.
- Saved record date range filtering for all dates, last 7 days, and last 30 days.
- Saved record deletion.
- JSON history export.
- Local demo data reset.

## Example Prompt

```text
Use AI Farm Copilot.

Scenario: vineyard
Crop: Cabernet Sauvignon
Block size: 1.2 hectares
Weather: hot week, no rain, windy afternoons
Irrigation: drip, last irrigated 3 days ago
Observation: lower leaves yellowing on several vines, some curling at edges
Photo: attached

Please generate an inspection report and next action plan.
```

## Repository Structure

```text
ai-farm-copilot/
  skills/ai-farm-copilot/     Agent skill package
  demo/                       Local browser demo
  examples/                   Scenario examples
  docs/                       Roadmap, safety, hardware notes
  data-templates/             CSV templates for field and sensor data
```

## First Supported Scenarios

| Scenario | First use case | Output |
| --- | --- | --- |
| Vineyard | Scout vine stress, leaf color, irrigation risk | Block inspection report |
| Orchard | Tree health, pest pressure, fruit stress | Orchard task plan |
| Golf turf | Turf discoloration, dry spots, compaction risk | Groundskeeping action list |
| Home garden | Plant diagnosis and care planning | Garden care plan |

## Roadmap

- V0: agent skill, examples, local demo, CSV templates.
- V0.1: image preview, richer reports, markdown export.
- V0.2: multi-image preview, sensor notes, local saved records, JSON history export.
- V0.3: managed area records and area-level inspection summaries.
- V0.4: monitoring dashboard and area health summaries.
- V0.5: local data management controls.
- V0.6: weather import and sample weather fallback.
- V0.7: photo role tagging and image intake checklist.
- V0.8: CSV import for sensor readings and inspection logs.
- V0.9: camera and drone photo batch workflow.
- V0.10: ESP32/Raspberry Pi sensor JSON adapter.
- V0.11: NDVI and map-based scouting notes.
- V0.12: Advisor Mode and 7-day care plan.
- V0.13: Browser print and Save as PDF report export.
- V0.14: Copyable advisor prompt export for Codex and Claude.
- V0.15: Scenario-specific advisor prompt templates.
- V0.16: Saved inspection risk trend chart.
- V0.17: Dashboard and trend filtering by managed area.
- V0.18: Dashboard risk filtering.
- V0.19: Saved record search.
- V0.20: Saved record sorting.
- V0.21: Saved record quick filters.
- V0.22: Per-area risk trend lines.
- V0.23: Area detail view.
- V0.24: Dashboard and saved record date range filters.
- V0.25: Browser geolocation for automatic coordinates.
- V0.26: Local timezone and inspection time.
- V0.27: 7-day weather forecast risk notes.
- V0.28: Local map view for current coordinates, managed areas, and saved inspection points.
- V0.29: Managed area boundary sketches attached to saved inspection records.
- V0.30: Satellite-style local basemap layer for clearer map context.
- V0.31: Satellite NDVI data and cloud-aware image selection for bounded areas.
- V0.32: Satellite NDVI time comparison and trend status.
- V1: hosted dashboard and optional hardware kit integrations.

See `docs/roadmap.md` for the full plan.

## Commercial Model

The core project is free and open source. Long-term commercial layers may include hosted dashboards, deployment support, camera/sensor kits, drone workflows, turf or vineyard reporting packages, and integrations with mowing robots, spray robots, tractors, and farm equipment platforms.

## License

MIT License. See `LICENSE`.
