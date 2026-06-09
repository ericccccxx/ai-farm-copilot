# my-farm-advisor Compatibility Notes

`borealBytes/my-farm-advisor` is a useful adjacent open-source farm advisor skill.

FarmGPT should not copy code from it directly. Instead, FarmGPT treats it as inspiration for a compatible advisor layer:

- FarmGPT focuses on monitoring workflows: managed areas, photos, weather, CSV/JSON sensor data, NDVI, saved records, and reports.
- Advisor-style output is implemented as FarmGPT's own `Advisor Mode`.
- Advisor Mode converts the current inspection state into decision-support guidance.

## Advisor Mode Output

FarmGPT Advisor Mode generates:

- Likely issue posture.
- Missing evidence.
- Data confidence.
- Next question to answer.
- Expert review trigger.
- 7-day care plan.

## Safety Boundary

Advisor Mode is not a certified agronomist, pesticide adviser, irrigation engineer, or compliance authority. It is for scouting support and decision preparation.

