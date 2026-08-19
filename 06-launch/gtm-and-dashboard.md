# GTM Strategy & Success Dashboard (Module 6)

## Get your prior work ready
- **The feature you're launching from your M4 PRD, one feature, not a list:** Spotlight Curated Rail, a hand-picked homepage rail of 3 to 5 titles, above the fold, mobile-first, visually distinct from algorithmic rows.
- **What your M5 experiment told you shipped / iterating, the evidence behind the launch:** Iterating, not yet shipped. The experiment was fully designed (hypothesis, control/variant, guardrails, shipping criteria) but the actual 90-day test had not yet run or returned results within this session, the baseline churn rate and final sample size remained unresolved pending real dashboard data. The evidence behind the launch is therefore the validated experiment design itself, a 15-point MDE grounded in an already-observed 22-point churn ceiling for Spotlight-exposed Wanderers, plus firm guardrails (Power User engagement ≥58%, Catalog Utilization stable), not a completed, data-confirmed ship decision.
- **Your persona pull your M2 persona, this anchors your audience:** Jamie Torres, 32, an active 18-month subscriber who distrusts StreamLine's recommendations and often turns to Reddit, friends, or a competitor app instead. M3 data later pointed to Wanderers, a lower-frequency, lower-LTV, more passive segment, as the higher-leverage target audience for this launch.

## Set your goal, then your audience
- **Primary GTM goal awareness · engagement · conversion, pick one:** Engagement
- **Why this goal? what makes this the right goal for this feature right now:** Wanderers are already subscribed and already opening the app, the gap isn't awareness of StreamLine, and there's no traditional conversion event here. The goal is shifting behavior from passive, low-trust browsing to active engagement with curated content, the lever that drives the churn reduction outcome.
- **Target audience the specific segment your goal implies, be precise:** Wanderers, 41% of the base, 1.1 sessions/week, lowest LTV ($8.40/month), 61% trending / 18% curated content mix, the segment showing the largest measurable engagement and churn response (22-point ceiling) to curated content exposure.

## Size your launch
- **Launch tier S (minimal) · M (targeted) · L (multi-channel) · XL (full GTM):** M- targeted
- **Justification reach + revenue impact + what silence would risk:** Reach: 41% of the base (Wanderers), though Phase 1 exposure is deliberately limited to a 50/50 split for controlled testing.

Revenue Impact: Low per-user value ($8.40 LTV) but meaningful in aggregate given the segment's size, a volume play, not a high-margin one.

Risk of Silence: High, an unclear or unmeasured result stalls validation of the entire Spotlight initiative's core hypothesis, leaving the Module 1 churn risk unaddressed for another quarter.
- **Is this a launch or a release? does it need go-to-market, or can it just ship?:** This is a Release, not a Launch, it ships internally to an existing segment with no external marketing, just controlled testing and minimal enablement.

## Choose your top three channels and plan assets
- **Channel 1 owned / earned / paid, and why it reaches your audience:** In-App Placement (Owned). Reaches Wanderers directly because it's embedded in the product itself, exposure happens automatically the moment they open the app, no separate action required to "find" the message.
- **Channel 2 owned / earned / paid, and why:** Targeted Push Notification (Owned). Reaches Wanderers specifically because it directly addresses their defining behavior, low session frequency (1.1x/week), by prompting a return visit rather than waiting for them to organically open the app.
- **Channel 3 owned / earned / paid, and why:** Internal Enablement Channel (Owned). Not customer-facing, reaches internal teams (content-ops, support, analytics) to keep everyone aligned on the same facts and metrics before, during, and after the test.
- **Enablement & assets what Sales / CS / Support need, plus the assets to build (one-pager, demo, etc.):** What Support/CS Need: A brief FAQ covering what the rail is and why some users see it and others don't (A/B context), enough to answer basic questions without a scripted campaign.

What Content-Ops Need: A one-page workflow guide for selecting and updating curated titles via direct data entry.

What Analytics Needs: A dashboard brief defining the primary metric, guardrails, and reporting cadence so all teams read the same numbers.

Assets to Build: One-pager (FAQ for Support), workflow guide (Content-Ops), dashboard brief (Analytics), and push notification copy (CRM/Push team). No demo needed, this is a homepage feature, not a sales-facing product requiring a walkthrough.

## Make it executable
- **Ownership named owner per key activity, individual, not department:** Build & rail deployment: Marcus, Engineering Lead
Visual design: Priya, Product Designer
Curated title selection/updates: Sofia, Content/Curation Lead
Push notification to lapsed Wanderers: James, CRM/Push Owner
Support FAQ & ticket monitoring: Derek, Support Lead
Guardrail checks & dashboard: Aisha, Analytics Lead
Day 30 checkpoint & Day 90 ship/iterate/kill decision: You, Product Manager, needs a named backup before lock
- **Budget & resource gaps what costs extra, and any asset you can't currently build:** Costs Extra: CRM/push infrastructure for lapsed Wanderers (needs sign-off), automated guardrail dashboard, and content curation tool, both deferred to Phase 3 if the initiative scales.

Can't Currently Build: A confirmed baseline churn rate (data gap, not budget), a content-team curation UI, and real-time automated guardrail monitoring, all substituted with manual workarounds for this sprint.

Bottom line: Phase 1 is fully resourced within the existing sprint; the real gaps only become costs if the initiative scales.
- **Timeline Phase 1 beta → Phase 2 launch moment → Phase 3 post-launch:** Phase 1, Beta (Weeks 1–3): Build, curate initial titles, prep enablement assets.

Phase 2, Launch Moment (Days 1–90): 50/50 test to Wanderers, push notification to lapsed users, weekly guardrail checks, Day 30 checkpoint, Day 90 ship/iterate/kill read.

Phase 3, Post-Launch (Day 91+): If shipped, expand to Casual Browsers, build deferred tools (content UI, automated guardrail dashboard) as scaling requires.

## Define how you'll know it worked
- **Success metrics 2 to 3 metrics that match your GTM goal:** Wanderer Segment Churn Rate (Primary), ≥15-point reduction, Spotlight-exposed vs. non-exposed
Rail Click-Through Rate (Engagement proxy), early signal of curated content resonance before churn data matures
Power User Curated Engagement Rate (Guardrail), must hold at ≥58%
- **Bad signal to watch for e.g. high reach, zero signups = message-market mismatch:** High reach with low clicks means the content itself isn't compelling. Churn improves but Power User engagement drops means you're breaking your best segment to fix another. Clicks are healthy but churn doesn't move means engagement isn't translating into retention.
- **Most likely post-launch decision double-down · iterate · pivot · deprioritize, and what would trigger it:** Iterate, most likely outcome. Trigger: Wanderer churn shows positive but sub-15-point movement, confirming curation works directionally but rail design, title selection, or placement needs refinement before scaling.

Double-down, if churn hits ≥15 points and guardrails hold, triggers Phase 3 expansion to Casual Browsers.

Pivot, if churn is flat despite healthy click-through, signals the mechanism (trust via curation) isn't the real lever, requiring a different hypothesis.

Deprioritize, if churn shows no movement and click-through is also low, signals Wanderers aren't responsive to this intervention at all.
