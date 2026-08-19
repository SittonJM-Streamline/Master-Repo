# A/B Experiment Brief, StreamLine (B2C)

## Parameters
| Parameter | Decision |
|---|---|
| Feature under test | Spotlight Curated Rail: 3 to 5 hand-picked titles, above the fold, mobile-first, visually distinct from algorithmic rows, with impression/click tracking, manually curated via direct data entry. |
| Persona | Jamie Torres, 32, an active 18-month subscriber who distrusts StreamLine's recommendations and often turns to Reddit, friends, or a competitor app instead. M3 data later pointed to Wanderers, a lower-frequency, lower-LTV, more passive segment, as the higher-leverage target. |
| Expected outcome | Final Answer:  Expected Outcome (M3, High-Level) Wanderers shift from passive, low-trust browsing to confidently selecting a title within the first minute of opening the app, reducing churn by at least 15 points without disrupting Power User engagement. |
| Primary success metric | A 15-percentage-point reduction in Wanderer Segment Churn Rate |
| Baseline rate | Not available. M3 data only reported the relative churn improvement for Wanderers under Spotlight exposure (22 points), not the standalone non-exposed Wanderer churn percentage. This figure still needs to be pulled from source dashboards before finalizing sample size calculations. |
| Guardrail metric | Power User Curated Content Engagement Rate, must stay at or above 58%. |
| Guardrail boundary | 58% (must not fall below this threshold) |
| Second guardrail | Catalog Title Utilization Rate, must not decline, protects against over-indexing engagement on just a few curated titles while the broader catalog goes even more undiscovered. |
| Minimum Detectable Effect | 15 percentage points, the minimum reduction in Wanderer churn (Spotlight-exposed vs. non-exposed) worth shipping. |
| Sample size per arm | 166 |
| Traffic split | 50/50 |
| Test duration | 90 days, with a guardrail check at Day 30 |
| Significance threshold | p < 0.05 (95% confidence level), the standard threshold, no deviation. |

## Control vs. Variant
- **Control (A):** The current homepage, algorithmic rows only, no curated rail. This produces the M2 Moment of Misery (60–90 second scroll, then exit) and the M3 funnel losses (29-point Homepage-to-Browse drop, 19-point Detail-to-Play drop, 11% reaching 30+ min sessions).
- **Variant (B):** add the Spotlight Curated Rail (3 to 5 hand-curated titles, above the fold, mobile-first, visually distinct from algorithmic rows) to the homepage. No other elements, algorithmic rows, navigation, or Power User pathways, are modified.
- **Held constant (isolation check):** Everything except the Spotlight rail stays identical: app version, recommendation engine, existing rows, navigation, onboarding, notifications, billing, and Power User pathways. Both arms run concurrently over the same 90-day window with identical external conditions. Any unrelated change hitting only one arm compromises attribution.

## Hypothesis
> I believe that Spotlight Curated Rail: 3 to 5 hand-picked titles, above the fold, mobile-first, visually distinct from algorithmic rows, with impression/click tracking, manually curated via direct data entry. for Jamie Torres, 32, an active 18-month subscriber who distrusts StreamLine's recommendations and often turns to Reddit, friends, or a competitor app instead. M3 data later pointed to Wanderers, a lower-frequency, lower-LTV, more passive segment, as the higher-leverage target. will result in Final Answer:  Expected Outcome (M3, High-Level) Wanderers shift from passive, low-trust browsing to confidently selecting a title within the first minute of opening the app, reducing churn by at least 15 points without disrupting Power User engagement., as measured by a 15 percentage points, the minimum reduction in Wanderer churn (Spotlight-exposed vs. non-exposed) worth shipping. change in A 15-percentage-point reduction in Wanderer Segment Churn Rate within 90 days, with a guardrail check at Day 30. We will protect Power User Curated Content Engagement Rate, must stay at or above 58%. throughout the test.

## Shipping criteria
> We will **ship** if A 15-percentage-point reduction in Wanderer Segment Churn Rate improves by ≥ 15 percentage points, the minimum reduction in Wanderer churn (Spotlight-exposed vs. non-exposed) worth shipping. at p < 0.05 (95% confidence level), the standard threshold, no deviation. and Power User Curated Content Engagement Rate, must stay at or above 58%. does not reach 58% (must not fall below this threshold) after 90 days, with a guardrail check at Day 30.
> We will **iterate** if direction is positive but lift is below the MDE.
> We will **kill** if the primary metric shows no improvement or moves negatively.
> The read date is fixed at the end of 90 days, with a guardrail check at Day 30, no results reviewed before this date.
