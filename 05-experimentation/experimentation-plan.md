# Experimentation Plan (Module 5)

## Get your documents ready
- **From M3, your hypothesis sentence:** Curated Spotlight placements will reduce churn among Wanderers, the largest, lowest-LTV, lowest-trust segment of the base, targeting at least a 15-point churn improvement, while protecting Power User curated engagement (58% baseline) as a guardrail. Go/no-go decision at 90 days, with an early check at Day 30.
- **From M3, your primary success metric & guardrail metric:** Primary: Wanderer churn rate, Spotlight-exposed vs. non-exposed, the segment most sensitive to curation's effect.

Guardrail: Power User curated engagement rate (58% baseline), protecting the platform's highest-LTV, lowest-churn segment from disruption.
- **From M4, the feature you scoped in your PRD this is what you're testing:** Spotlight Curated Rail, a hand-picked homepage row of 3 to 5 titles, above the fold, mobile-first, designed to give Wanderers a trustworthy pick the moment they open the app.

## Define your experiment parameters
- **Feature under test pull from your M4 PRD:** Spotlight Curated Rail

A hand-picked homepage rail that bypasses the algorithm entirely, surfacing 3 to 5 human-curated titles the moment a user lands on the homepage, above the fold, mobile-first, requiring no scrolling before a trustworthy title is visible. Titles are set via direct data entry (no content-team UI in this build), and the rail is visually distinct from existing algorithmic rows to signal human curation rather than algorithmic guessing.
- **Persona pull your M2 persona:** data later revealed Wanderers, a lower-frequency, lower-LTV, more passive segment, as the higher-leverage target, though Jamie remains the original qualitative anchor.
- **Expected outcome the behaviour change you expect, from your M3 hypothesis:** Wanderers exposed to the Spotlight Curated Rail shift from passive, low-trust browsing, relying on trending content and often abandoning sessions without watching, to confidently selecting a title within the first minute of opening the app. This behavior change is expected to reduce Wanderer churn by at least 15 points relative to non-exposed Wanderers, while Power User curated engagement remains stable at or above 58%, confirming the shift doesn't come at the cost of the platform's healthiest segment.
- **Primary success metric the one number that defines success, from M3:** Target: at least a 15-point reduction in churn for Spotlight-exposed Wanderers relative to non-exposed Wanderers, building toward the 22-point ceiling already observed in prior Spotlight-exposed Wanderer cohorts.
- **Baseline rate today's rate of your primary metric, from your M3 data:** The M3 data provided only the relative churn improvement for Wanderers under Spotlight exposure, a 22-point reduction, not the actual standalone baseline churn percentage. That specific number wasn't part of the data reviewed and would need to be pulled from source dashboards before finalizing this experiment parameter.
- **Guardrail metric & boundary what must not break, and how far it can move before you investigate:** Power User curated engagement must stay at or above 58%. Any drop triggers investigation; a sustained drop past Day 30 halts the test.
- **Minimum Detectable Effect (MDE) the smallest improvement worth shipping, your floor:** A 15-point reduction in Wanderer churn (Spotlight-exposed vs. non-exposed) is the floor, the smallest improvement worth shipping.

This threshold was already established in the Decision Rule: results below 15 points are treated as directionally positive but insufficient to scale, triggering iteration on rail design rather than a ship decision, while 15+ points justifies moving forward, building toward the 22-point ceiling observed in earlier Spotlight-exposed cohorts.
- **Sample size per arm use the calculator in the builder, baseline + MDE:** A standard two-proportion sample size calculation typically needs:

Baseline conversion rate (your non-exposed Wanderer churn rate, once you pull that exact figure from source data)
Minimum Detectable Effect (15 points, as defined)
Statistical significance level (commonly 95%)
Statistical power (commonly 80%)
- **Traffic split & test duration 50/50 standard · cover ≥ 2 weekly cycles:** Traffic Split: 50/50, Wanderers randomly assigned at the account level to Control (existing homepage, no Spotlight rail) or Treatment (homepage with Spotlight Curated Rail), preventing cross-contamination within a single user's sessions.

Test Duration: 90 days total, covering well over 2 full weekly cycles to smooth out day-of-week viewing pattern variance (e.g., weekend binge behavior vs. weekday casual browsing). A mandatory interim checkpoint at Day 30 confirms the guardrail is holding and early directional movement exists before continuing to full term.
- **Significance threshold p < 0.05 is standard, explain any deviation:** p < 0.05 (95% confidence level), the standard threshold, applies here with no deviation.

No adjustment is warranted for this test: it's a single primary metric (Wanderer churn) with one clearly defined guardrail (Power User engagement) evaluated independently, not a multi-comparison scenario where corrections like Bonferroni would be needed. The 90-day duration and 50/50 split are already designed to reach adequate statistical power at this standard threshold, so tightening or loosening it isn't justified by the experiment's design or stakes.

## Define your control and variant
- **Control (A) the current experience, reference your M2 moment of misery and M3 funnel/workflow data:** The current homepage, algorithmic rows only, no curated rail. This is the exact experience producing the Moment of Misery from M2 (60 to 90 second scroll, then exit) and the funnel losses from M3 (29-point Homepage-to-Browse drop, 19-point Detail-to-Play drop, 11% reaching 30+ min sessions).
- **Variant (B) your single change, copy the relevant screens & functional requirements from your M4 PRD:** One change only: add the Spotlight Curated Rail (3 to 5 hand-curated titles, above the fold, mobile-first, visually distinct from algorithmic rows) to the homepage. Impressions and clicks are tracked; no other homepage elements, algorithmic rows, or Power User pathways are modified.
- **Isolation check, what has NOT changed? list everything identical between arms (app version, recommendation engine, notifications, onboarding). If something changed inadvertently, your test is compromised.:** Everything except the Spotlight rail stays identical: app version, recommendation engine, existing rows, navigation, onboarding, notifications, billing, and Power User pathways. Both arms run concurrently over the same 90-day window with identical external conditions. Any unrelated change hitting only one arm compromises attribution.

## Formalize your hypothesis & shipping criteria
- **Your hypothesis (filled in):** I believe that the Spotlight Curated Rail for Wanderers will result in increased confidence to select a title within the first minute of opening the app, rather than abandoning the session or exiting to an external source, as measured by a 15 percent change in Wanderer Segment Churn Rate (Spotlight-exposed vs. non-exposed) within a 90-day test duration. We will protect Power User Curated Content Engagement Rate (58% baseline) throughout the test.
- **Your shipping criteria (filled in):** Ship if Wanderer churn improves by 15+ points at p < 0.05, and Power User engagement holds at or above 58%.

Iterate if the lift is positive but under 15 points.

Kill if there's no improvement or a negative move.

Decision locked in at the 90-day mark, no early peeking.
- **Hardest parameter to define, and did it change your hypothesis? quick debrief:** The Baseline Rate was the hardest parameter to define, and it exposed a real gap rather than just a technical annoyance.

Throughout Module 3, the segmentation data gave a clean, compelling number: a 22-point churn improvement for Spotlight-exposed Wanderers. That number was strong enough to anchor the entire hypothesis, the MDE, the shipping criteria, even the persona pivot from Jamie to Wanderers. But when it came time to actually size the experiment, plug numbers into the sample size calculator, I realized the relative improvement (22 points) and the standalone baseline (what percentage of non-exposed Wanderers churn today) are two different numbers, and only the second one is usable as a calculator input.

This is exactly the trap called out earlier in this process, don't conflate the primary metric with other numbers that look similar but answer different questions. A relative lift tells you the treatment effect size; the calculator needs the untreated starting point to determine how many users you need to detect that effect reliably.

Did it change the hypothesis? Not the hypothesis itself, the 15-point MDE and the 22-point ceiling both remained valid and well-supported. But it did change my confidence in being "done." It surfaced a dependency I couldn't resolve from the data already reviewed, I had to explicitly flag that the actual baseline churn percentage needed to be pulled from source dashboards before the sample size and, by extension, the real feasibility of hitting significance in 90 days, could be finalized.

The honest takeaway: A hypothesis can feel fully formed on the strength of a relative effect size, but shipping criteria and sample sizing demand an absolute number. That gap between "directionally validated" and "operationally ready to test" is easy to miss until you're the one filling in the calculator field.
