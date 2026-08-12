# Feature Roadmap, Module 4 · StreamLine Spotlight

**Team:** 2 engineers + 1 designer

## Strategic anchors
- **Persona:** The Wanderer
- **Primary metric:** Wanderer Segment Churn Rate, Spotlight-Exposed vs. Non-Exposed  This is the leading indicator because it directly reflects the mechanism the entire hypothesis rests on, curation reducing churn in the segment with the greatest observed sensitivity to it.
- **Moment of misery:** The browsing experience offers no trustworthy signal to distinguish a worthwhile title from the noise of 15,000 undifferentiated options  forcing Jamie to either gamble on an unproven pick or abandon the app entirely to find that trust elsewhere.  Jamie opens StreamLine intending to find something to watch. They scroll through the same recurring rows "Trending," "Popular," "Because You Watched X"  for 60–90 seconds. Nothing stands out as credible or personally relevant; every row feels like a guess rather than a recommendation. Rather than risk 20+ minutes on an unproven title, Jamie exits the app to Google, Reddit, or a text to a friend outsourcing the exact job StreamLine was supposed to do.
- **Guardrail:** Power User Curated Content Engagement Rate (currently 58% curated / 22% trending)  This is the guardrail because Power Users already represent the platform's healthiest, highest-LTV segment ($14.20 avg monthly LTV, 4.8 sessions/week, effectively zero churn), and any shift in Spotlight design aimed at improving Wanderer outcomes must not disrupt what is already working for this base.

## Scoring
| Feature | Value | Effort | Quadrant | Decision | Rationale |
|---|---|---|---|---|---|
| A1 Spotlight Curated Rail | 5 | 2 | Quick Win | Next | Value increases. This is the lowest-effort, highest-fit intervention for the Wanderer's actual moment of misery, a passive homepage entry point that requires zero user effort, directly targeting the 29-point Homepage-to-Browse drop |
| A2 'Why You'll Love This' Label | 3 | 4 | Time Sinker | Next | Both scores move against it. Value drops because hover-based explanation assumes active title inspection, more a Jamie/Power User behavior than a passive Wanderer's. Effort rises sharply because it's an AI-generation feature, and critically, hover doesn't function on the mobile-first base this platform actually serves (DAU data confirms mobile is the dominant surface) |
| A3 Hidden Gem Badge | 2 | 2 | Fill-In | Later | Value drops slightly. Surfacing low-viewcount, high-quality titles assumes a willingness to explore beyond trending content, the opposite of the Wanderer's confirmed 61% trending reliance |
| A4 Mood-Based Entry Point | 5 | 4 | Major Project | Next | Value rises, this is a near-zero-effort-for-user entry mechanic, ideal for a passive persona. Effort also rises because mood-tagging the full catalog is real engineering and content-ops lift, likely exceeding a single 3-week sprint for a 2-engineer team, flag as a scope risk, not a clean single-sprint item |
| A5 Personalized Spotlight Queue | 5 | 5 | Major Project | Next | Unchanged in score, but add an explicit capacity flag: with 2 engineers and 3 weeks, this is not realistically shippable in one sprint. Recommend explicitly phasing it rather than scoring it as sprint-ready |
| A6 Spotlight Digest Email | 3 | 1 | Fill-In | Later | Value increases meaningfully. Wanderers are defined by low session frequency (1.1x/week), meaning an outside-the-app re-engagement channel may be more valuable for this specific persona than for higher-frequency segments, this was undervalued originally |
| A7 Curator Profiles | 1 | 1 | Fill-In | Later | Unchanged. Following curators requires active, parasocial engagement, contrary to the Wanderer's passive behavior. Correctly deprioritized |
| A8 Watch Party (Spotlight) | 1 | 1 | Fill-In | Later | Unchanged. No connection to the discovery-trust friction driving the hypothesis |
| A9 Advanced Filter Engine | 2 | 2 | Fill-In | Now | Value drops significantly. Filtering by decade/language/runtime assumes the user already knows what they want, active-search behavior far closer to Power Users than Wanderers. This item's original "Now" placement appears driven by Engineering's preference, which your prompt explicitly instructs me to deprioritize |
| A10 Offline Download (Spotlight) | 2 | 3 | Time Sinker | Cut | Value drops slightly. No tie to the churn hypothesis, Sales-requested without data support, correctly cut either way |

## Roadmap
### NOW, 3-week sprint
- **A9 Advanced Filter Engine**, Value drops significantly. Filtering by decade/language/runtime assumes the user already knows what they want, active-search behavior far closer to Power Users than Wanderers. This item's original "Now" placement appears driven by Engineering's preference, which your prompt explicitly instructs me to deprioritize

### NEXT, following 1-2 sprints
- **A1 Spotlight Curated Rail**, Value increases. This is the lowest-effort, highest-fit intervention for the Wanderer's actual moment of misery, a passive homepage entry point that requires zero user effort, directly targeting the 29-point Homepage-to-Browse drop
- **A2 'Why You'll Love This' Label**, Both scores move against it. Value drops because hover-based explanation assumes active title inspection, more a Jamie/Power User behavior than a passive Wanderer's. Effort rises sharply because it's an AI-generation feature, and critically, hover doesn't function on the mobile-first base this platform actually serves (DAU data confirms mobile is the dominant surface)
- **A4 Mood-Based Entry Point**, Value rises, this is a near-zero-effort-for-user entry mechanic, ideal for a passive persona. Effort also rises because mood-tagging the full catalog is real engineering and content-ops lift, likely exceeding a single 3-week sprint for a 2-engineer team, flag as a scope risk, not a clean single-sprint item
- **A5 Personalized Spotlight Queue**, Unchanged in score, but add an explicit capacity flag: with 2 engineers and 3 weeks, this is not realistically shippable in one sprint. Recommend explicitly phasing it rather than scoring it as sprint-ready

### LATER, backlog
- **A3 Hidden Gem Badge**, Value drops slightly. Surfacing low-viewcount, high-quality titles assumes a willingness to explore beyond trending content, the opposite of the Wanderer's confirmed 61% trending reliance
- **A6 Spotlight Digest Email**, Value increases meaningfully. Wanderers are defined by low session frequency (1.1x/week), meaning an outside-the-app re-engagement channel may be more valuable for this specific persona than for higher-frequency segments, this was undervalued originally
- **A7 Curator Profiles**, Unchanged. Following curators requires active, parasocial engagement, contrary to the Wanderer's passive behavior. Correctly deprioritized
- **A8 Watch Party (Spotlight)**, Unchanged. No connection to the discovery-trust friction driving the hypothesis

### ✂ Cut List
- **A10 Offline Download (Spotlight)**, Value drops slightly. No tie to the churn hypothesis, Sales-requested without data support, correctly cut either way
