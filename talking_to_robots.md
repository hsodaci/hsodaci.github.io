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

Two controlled experiments, run as part of my PhD, that use the same logic growth teams use to test product changes: comparing conditions, measuring a behavioral outcome, and asking what actually moved it. The audience was a robot instead of a landing page, but the method is identical: hold everything constant except the variable under test, then look at what people actually did, not what they said they'd do.

<div class="case-block">
  <div class="case-block-label">The problem</div>
  <p>When someone interacts with a new system — a robot, an app, an onboarding flow — they don't know upfront how much it "gets." They give more explanation than needed, then adjust based on signals of success or failure. Which signals actually change behavior, and which ones people just assume should work, is an empirical question.</p>
</div>

<div class="case-block">
  <div class="case-block-label">What I built to measure it</div>
  <p>I built a custom metric, <strong>semantic detail density</strong>: the number of distinct, meaning-relevant pieces of information a person included in a response. It's a proxy for a general growth question — how much convincing does a user think they still need to do — and it's more sensitive than a surface metric like message length.</p>
</div>

<div class="case-step">
  <div class="case-step-number">1</div>
  <div class="case-step-body">
    <h3 class="case-step-title">Audience A/B test</h3>
    <p>Participants described words to either a human or a robot listener, using prerecorded video so timing and accuracy stayed identical across both conditions and only who was listening varied.</p>
    <div class="case-result">
      <span class="case-result-label">Result</span>
      People gave the robot more detail than the human, consistently, and didn't scale it back even after the robot got several answers right in a row. Task success alone wasn't a strong enough signal to change behavior. This became a published paper at ACM/IEEE HRI '26, which received an Honorable Mention.
    </div>
  </div>
</div>

<div class="case-step">
  <div class="case-step-number">2</div>
  <div class="case-step-body">
    <h3 class="case-step-title">Feedback multivariate test</h3>
    <p>The multivariate equivalent of Test 1's single-variable design: I tested two signals from the robot together instead of one at a time. <strong>Framing</strong> — did the robot open by claiming competence, or say nothing about its ability? <strong>Feedback</strong> — on a correct guess, did it give specific praise, or just a bare acknowledgment?</p>
    <div class="case-result">
      <span class="case-result-label">Result</span>
      Neither signal, nor the combination, moved the metric. People didn't give less detail just because the system claimed competence or praised them. But a signal we hadn't tested as a primary hypothesis did: when the robot explicitly said it failed and asked for another try, people immediately added more detail on the next response, then reverted back to baseline right after.
    </div>
  </div>
</div>

<div class="case-insight">
  <div class="case-insight-label">What this means for a growth context</div>
  <p>The pattern that held across both experiments: <strong>vague positive signals don't change behavior; specific, actionable signals do.</strong> Telling a user something worked, or that the system is capable, doesn't reliably shift what they do next. Telling them specifically what didn't work — in a moment they can still act on it — does, immediately and measurably. Applied to funnels and paywalls: generic encouragement in an upsell or onboarding step is unlikely to move behavior on its own; specific, actionable feedback at the point of friction is where the effect actually is.</p>
</div>

<div class="pub-actions">
  <a class="pub-btn pub-doi" href="/academia/">Full write-ups &amp; citations</a>
</div>

**Tools:** R, custom behavioral coding, reproducible analysis
