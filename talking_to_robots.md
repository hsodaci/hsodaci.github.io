---
title: Talking to Robots
permalink: /projects/talking-to-robots/
layout: page
excerpt: Two controlled experiments on what actually changes user behavior — reframed as an A/B test and a multivariate test.
comments: false
---

<p class="pub-meta">PhD dissertation research, reframed as a growth case study &middot; Koç University &middot; 2020–2026</p>

<div class="pub-tags">
  <span class="pub-tag">A/B Testing</span>
  <span class="pub-tag">Multivariate Testing</span>
  <span class="pub-tag">Behavioral Analytics</span>
  <span class="pub-tag">R</span>
  <span class="pub-tag">Experimental Design</span>
</div>

Two controlled experiments, run as part of my PhD, that use the same logic growth teams use to test product changes — comparing conditions, measuring a behavioral outcome, and asking what actually moved it. The audience was a robot instead of a landing page, but the method is identical: hold everything constant except the variable under test, then look at what people actually did, not what they said they'd do.

<div class="pub-actions">
  <a class="pub-btn pub-doi" href="/academia/">Academia page (papers &amp; DOIs)</a>
</div>

#### Situation

When someone interacts with a new system — a robot, an app, an onboarding flow — they don't know upfront how much it "gets." They give more explanation than needed, then adjust based on signals of success or failure. Which signals actually change behavior, and which ones people just say they're paying attention to, is an empirical question, not something you can assume from a UX brief.

#### Task

Measure the thing that actually matters — how much information a person volunteers before they trust the system understood them — and test which conditions move that metric versus which ones only feel like they should.

I built a custom behavioral metric for this, **semantic detail density**: the number of distinct, meaning-relevant pieces of information a person included in a response (validated for inter-rater reliability, ICC = .853). It's a proxy for a general growth question — how much convincing does a user think they still need to do — that's more sensitive than surface metrics like message length.

#### Action — Test 1: audience A/B test

Structured like an A/B test with two arms instead of one control: 55 participants described words to either a human or a robot listener (video-based, response timing and accuracy fixed identically across both arms so only "who's listening" varied). The dependent variable was semantic detail density per trial, modeled with mixed-effects and cumulative-link models in R across 2,640 trials.

**Result:** People gave the robot more detail than the human, consistently, and — unlike with the human — didn't scale it back even after the robot got several answers right in a row. Task success alone wasn't a strong enough signal to change behavior. This became a [published paper at ACM/IEEE HRI '26](/academia/), which received an Honorable Mention.

#### Action — Test 2: feedback multivariate test

A 2×2 between-subjects test (96 participants, 3,200 trials) — the multivariate equivalent of Test 1's single-variable A/B design. Two "treatments" were crossed independently:

- **Framing:** did the robot open by claiming competence ("I've been trained on millions of words") or say nothing about its ability?
- **Feedback:** on a correct guess, did it give specific praise ("very clear") or just a bare "okay"?

**Result:** Neither treatment, nor their interaction, moved the metric — people didn't give less detail just because the system claimed competence or praised them. But a signal we hadn't tested as a primary hypothesis did: when the robot explicitly said it *failed* and asked for another try, people immediately added more detail on the very next response (OR = 2.14, p < .001) — then reverted back to baseline right after.

#### What this means for a growth context

The pattern that held across both experiments: **vague positive signals don't change behavior; specific, actionable signals do.** Telling a user something worked, or that the system is capable, doesn't reliably shift what they do next. Telling them specifically what didn't work — in a moment they can still act on it — does, immediately and measurably. Applied to funnels and paywalls: generic encouragement in an upsell or onboarding step is unlikely to move behavior on its own; specific, actionable feedback at the point of friction is where the effect actually is. That's the kind of result you only get by testing the vague-vs-specific distinction directly instead of assuming positive messaging works.

**Tools/methods:** R (mixed-effects & cumulative link models), custom behavioral coding scheme, Choregraphe (robot programming), reproducible analysis pipelines
**Full write-ups, DOIs, and citations:** see the [academia](/academia/) page
