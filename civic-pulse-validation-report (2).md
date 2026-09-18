# Prototype & Validation Report — Civic Pulse
### Pathway A — Continuation Track

## 1. Problem Statement (carried forward)
Residents have no reliable channel to report civic issues (potholes, water leaks, streetlight faults, garbage) — complaints go into busy phone lines or paper registers with no tracking number, so people give up reporting. Meanwhile, municipal teams that do receive reports see them in arrival order rather than risk order, so a minor complaint can sit ahead of a genuinely dangerous one (e.g. an exposed live wire near a school).

## 2. The Prototype
**Civic Pulse** is a working digital prototype with two sides:
- **Citizen portal:** file a report (category, location, description, optional photo), track your own reports, view a community board sorted by urgency, see a leaderboard/badges for civic participation.
- **Admin panel:** a triage dashboard showing open work orders ranked by an urgency score, category and zone breakdowns, department assignment, status updates, and internal notes.

**How urgency scoring works:** a lightweight, explainable heuristic — category base risk (e.g. water leak/exposed wire scored higher than garbage), risk-language detection in the description (words like "accident," "school," "children"), and duplicate clustering so repeat reports corroborate an existing ticket instead of creating noise.

Fidelity: fully clickable, functional prototype (no backend — session-only, browser-based), so testers experience the actual flow rather than static mockups.

## 3. Testing Method
- **Testers:** 3 new testers
- **Method:** sent the live prototype link directly (via text), asked each person to try filing a report as a citizen and explore the admin view, then share their reaction.
- **Date(s):** 17/09/2026

## 4. Tester Feedback

| Tester | Reaction |
|---|---|
| Tester 1 | "Ooh this actually looks legit, not like a college project mock-up. The priority scoring and zone heatmap thing is a nice touch." |
| Tester 2 | "The design language is solid — that stamped 'SAMPLE' ticket and the whole industrial/blueprint vibe fits a civic reporting app well. Would love to see how it handles duplicate reports though." |
| Tester 3 | "Not gonna lie I'd actually use something like this if my area had it 😭 potholes near my house have been there for MONTHS lol." |

## 5. Key Themes from Feedback
All three testers reacted positively to the visual design and how quickly it communicated the app's purpose — one explicitly noted it didn't feel like a typical student mock-up. The urgency scoring and zone heatmap on the admin side stood out as the most memorable feature. Tester 2's interest in duplicate-handling shows the triage logic prompted genuine curiosity rather than confusion. Tester 3's response validated the core problem: real, unresolved civic issues (a pothole sitting for months) are exactly the friction the prototype targets, and the reaction suggests real intent to use it if it existed for their area.

## 6. Changes Made / Planned Based on Feedback
- Surface the duplicate-detection logic more visibly in the citizen-facing view (currently only explained on the homepage "How it works" section) — Tester 2's question suggests users are curious how their report interacts with existing ones, not just confused by its absence.
- Consider a short in-app note near the photo-attach field clarifying that this is a prototype and nothing leaves the browser, so expectations are set upfront.

## 7. Reflection
Testing with real people surfaced something a self-review wouldn't have: the design language itself was doing real work — it made the tool feel credible rather than like a class exercise, which mattered as much as the functionality to how testers judged it. It also confirmed the underlying problem is genuinely felt (a months-old pothole), not just an assumed one. If iterating further, the next step would be validating the urgency-scoring logic itself with a municipal-side user, since citizen-side feedback alone doesn't test whether the triage actually helps someone doing the fixing.
