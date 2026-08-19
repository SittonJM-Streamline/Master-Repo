# GTM Launch Plan, StreamLine (B2C)

| Field | Value |
|---|---|
| Feature | Spotlight Curated Rail, a hand-picked homepage rail of 3 to 5 titles, above the fold, mobile-first, visually distinct from algorithmic rows, manually curated via direct data entry, with impression/click tracking. |
| Goal | Engagement |
| Launch tier | M, Targeted |

## Goal & Audience
- **Goal:** Engagement, 1. The feature lives entirely inside the existing product. Spotlight isn't a new product or market entry, it's a homepage change for people who already have accounts and already open the app. There's no external audience to make aware of anything, which rules out Awareness as the goal.

2. There's no purchase or sign-up event to optimize toward. The feature doesn't ask a user to buy, upgrade, or convert in any transactional sense, it asks them to trust a recommendation and press play. That's a behavioral shift, not a conversion event, which rules out Conversion as the goal.

3. The M2/M3 evidence points specifically to a trust-and-behavior gap, not a discovery gap. Wanderers already know StreamLine exists and already open the app occasionally, their problem is that once inside, nothing earns enough trust to commit to watching. Engagement, measured through curated content interaction, directly targets that specific gap, which is why it's also the metric most tightly coupled to the M5 experiment's primary success measure (Wanderer churn, itself a downstream result of improved engagement).
- **Target audience:** Jamie Torres, 32, an active 18-month subscriber who distrusts StreamLine's recommendations and often turns to Reddit, friends, or a competitor app instead. M3 data later pointed to Wanderers, a lower-frequency, lower-LTV, more passive segment, as the higher-leverage target audience for this launch.

## Launch Tier
- **M, Targeted**, This is a Medium launch: small in engineering footprint and immediate revenue impact, but medium-to-high in strategic importance, because the real cost of getting the size wrong isn't wasted budget, it's a missed or noisy read on the single hypothesis the entire Spotlight initiative depends on.

## Channels
1. **Owned: Push Notification (Owned) — reaches lapsed Wanderers where they already are, outside the app, since their low session frequency (1.1x/week) means in-app placement alone can't reach the portion who aren't currently opening the app.**
2. **Earned: Not applicable. This release uses only owned channels. There is no Earned or Paid channel in this plan, adding one would misalign with the Engagement goal and the existing-subscriber audience already defined.**
3. **Paid: There is no Paid channel in this plan, adding one would misalign with the Engagement goal and the existing-subscriber audience already defined.**

## Enablement & Assets
What Support/CS Need: A brief FAQ covering what the rail is and why some users see it and others don't (A/B context), enough to answer basic questions without a scripted campaign.

What Content-Ops Need: A one-page workflow guide for selecting and updating curated titles via direct data entry.

What Analytics Needs: A dashboard brief defining the primary metric, guardrails, and reporting cadence so all teams read the same numbers.

Assets to Build: One-pager (FAQ for Support), workflow guide (Content-Ops), dashboard brief (Analytics), and push notification copy (CRM/Push team). No demo needed, this is a homepage feature, not a sales-facing product requiring a walkthrough.

## Ownership, Budget & Timeline
- **Ownership & budget:** Costs Extra:

CRM/push infrastructure for the lapsed-Wanderer segment, James needs sign-off from the CRM platform owner before assuming this is covered under existing tooling
Automated guardrail dashboard, explicitly deferred; becomes a real cost only if Phase 3 scaling proceeds
Content curation tool, deferred; becomes a cost only if refresh cadence exceeds what Sofia's manual entry can sustain
Asset Gaps (Can't Currently Build):

Confirmed baseline Wanderer churn rate, a data-access gap, not a budget one, still pending from M5
Content-team-facing curation UI, substituted this sprint with direct data entry
Real-time automated guardrail monitoring, substituted this sprint with Aisha's manual weekly check
One Accountability Gap to Flag: You are the sole named owner for both the Day 30 and Day 90 decisions. Before locking this plan, name a backup decision-maker in case you're unavailable at either checkpoint, this is the single point of failure in an otherwise fully-owned plan.
- **Timeline:** Phase 1, Beta (Weeks 1–3) Marcus builds the rail per M4 scope, Priya finalizes visual distinction treatment, Sofia populates the initial curated title set via direct data entry, and Derek, Aisha, and James draft their respective enablement assets (FAQ, dashboard brief, push copy).

Phase 2, Launch Moment (Days 0–90) Marcus deploys the 50/50 Control/Variant split to Wanderers on Day 0; James sends the push notification to lapsed Wanderers the same day. Aisha runs weekly guardrail checks throughout. You hold the Day 30 checkpoint to confirm guardrail health and early directional signal, then the Day 90 ship/iterate/kill decision, with Aisha's sign-off.

Phase 3, Post-Launch (Day 91+) If shipped, expand to Casual Browsers, and revisit the deferred content curation tool and automated guardrail dashboard as scaling demands. If iterating, redesign the rail based on sub-target results. If killed, document learnings and close out the experiment.

## Success Metrics
- **Metrics:** Wanderer Segment Churn Rate (Primary), ≥15-point reduction, Spotlight-exposed vs. non-exposed, by Day 90
Rail Click-Through Rate (Engagement proxy), early signal of curated content resonance before churn data matures
Power User Curated Engagement Rate (Guardrail), must hold at ≥58%, protects against solving one segment's problem by breaking another's experience
- **Bad signal to watch for:** High reach with low clicks means the content isn't compelling. Churn improves but Power User engagement drops means you're breaking your best segment to fix another. Clicks are healthy but churn doesn't move means engagement isn't translating into retention.
- **Likely post-launch decision:** Iterate is most likely, positive but sub-target churn improvement. Double-down if results hit the 15-point target with guardrails holding. Pivot if churn stays flat despite healthy click-through. Deprioritize if both churn and engagement are weak.
