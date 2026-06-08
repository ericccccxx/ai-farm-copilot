# Hardware Integration Notes

AI Farm Copilot should remain hardware-agnostic. The open-source core should accept photos and structured data from many sources.

## First Data Sources

- Phone photos.
- Manual field notes.
- CSV weather logs.
- CSV soil moisture logs.
- Drone photo folders.
- ESP32 or Raspberry Pi sensor JSON.

## Low-Cost Camera Path

First practical setup:

- Phone camera for manual scouting.
- Action camera or small RGB camera on a pole, cart, mower, or drone.
- Optional Raspberry Pi camera for fixed-location monitoring.

Recommended metadata:

- Date and time.
- Location, block, hole, bed, or row.
- Camera source.
- Crop, turf, or plant type.
- Weather summary.
- Notes from the operator.

## Sensor Path

Useful starter readings:

- Soil moisture.
- Air temperature.
- Humidity.
- Rainfall.
- Light level.
- Battery level.

Keep the first sensor adapter simple. JSON is enough:

```json
{
  "timestamp": "2026-06-08T08:30:00+08:00",
  "location": "vineyard-block-a",
  "soil_moisture_percent": 28,
  "air_temperature_c": 31,
  "humidity_percent": 46,
  "battery_percent": 82
}
```

## Drone Path

First workflow:

1. Capture overhead or angled RGB images.
2. Name photos by date and block.
3. Upload images with notes.
4. Ask the agent to compare affected and healthy areas.
5. Generate a scouting report.

NDVI can be added later, but the first version should not depend on it.

