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

The V0.4 demo supports:

- Local multi-image upload and preview.
- Managed area records for vineyard blocks, orchard sections, golf zones, and garden beds.
- Monitoring dashboard with area counts, record counts, high-risk count, and latest risk.
- Area health cards with risk bars and recent inspection status.
- Scenario-specific defaults for vineyard, orchard, golf turf, and home garden.
- Sensor and weather reading notes.
- Dynamic risk level and follow-up timing.
- Structured report generation.
- Markdown report download.
- Local saved inspection records.
- JSON history export.

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
- V0.5: image intake checklist and weather API adapter.
- V0.6: camera and drone photo batch workflow.
- V0.7: ESP32/Raspberry Pi sensor JSON adapter.
- V0.8: NDVI and map-based scouting notes.
- V1: hosted dashboard and optional hardware kit integrations.

See `docs/roadmap.md` for the full plan.

## Commercial Model

The core project is free and open source. Long-term commercial layers may include hosted dashboards, deployment support, camera/sensor kits, drone workflows, turf or vineyard reporting packages, and integrations with mowing robots, spray robots, tractors, and farm equipment platforms.

## License

MIT License. See `LICENSE`.
