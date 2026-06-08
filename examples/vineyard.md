# Example: Vineyard Inspection

## User Input

Scenario: vineyard  
Crop: Cabernet Sauvignon  
Block size: 1.2 hectares  
Weather: hot week, no rain, windy afternoons  
Irrigation: drip, last irrigated 3 days ago  
Observation: lower leaves yellowing on several vines, some curling at the edges  
Photo: attached by user  

## Expected Agent Output

# Inspection Report

## Context

- Scenario: Vineyard
- Managed area: Cabernet Sauvignon block
- Area size: 1.2 hectares
- Weather: Hot and dry week with wind
- Irrigation: Drip, last irrigation 3 days ago
- Recent treatment: Not provided

## Observations

- Lower leaves are yellowing on several vines.
- Some leaves are curling at the edges.
- The issue may be localized or spreading; pattern is not yet confirmed.

## Likely Causes

| Cause | Likelihood | Evidence | What to check next |
| --- | --- | --- | --- |
| Water stress | Medium | Heat, wind, and leaf curling | Compare soil moisture in affected and healthy rows |
| Nutrient deficiency | Medium | Lower leaf yellowing can match nutrient stress | Compare older and newer leaves; review fertilizer history |
| Irrigation uniformity issue | Medium | Symptoms on several vines may follow drip line variation | Check emitters and pressure in affected zone |
| Pest or disease pressure | Low to Medium | Not enough visual detail yet | Inspect underside of leaves and nearby vines |

## Risk Level

**Overall risk:** Medium

Reason: the issue is visible on multiple vines and weather stress is present, but the pattern and spread are not yet confirmed.

## Recommended Next Actions

1. Check soil moisture at root depth in affected and healthy vines.
2. Inspect drip emitters near affected vines.
3. Photograph underside of affected leaves and a healthy comparison vine.
4. Review recent fertilizer and spray history.
5. Recheck the same vines in 48-72 hours.

## Do Not Do Yet

- Do not apply chemical treatment based only on current evidence.
- Do not make a large irrigation change until emitter performance and soil moisture are checked.

