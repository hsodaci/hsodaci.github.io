---
title: Talking to Robots
permalink: /projects/talking-to-robots/
layout: page
excerpt: Two controlled experiments on communication and system design — reframed as an A/B test and a multivariate test.
comments: false
---

<p class="pub-meta">PhD dissertation research on communication and system design &middot; Koç University &middot; 2020–2026</p>

<div class="pub-tags">
  <span class="pub-tag">A/B Testing</span>
  <span class="pub-tag">Multivariate Testing</span>
  <span class="pub-tag">Behavioral Analytics</span>
  <span class="pub-tag">R</span>
  <span class="pub-tag">Experimental Design</span>
</div>

How much should a conversational partner explain itself before the person talking to it trusts it understood them? Too little, and people fill in the gaps themselves. Too much, and they stop listening.

I spent several years studying this question through two controlled experiments, then decided to bring that experimental mindset into product work, where a finding can change something for real users in weeks instead of years.

<div class="case-block">
  <div class="case-block-label">Why a robot, of all things</div>
  <p>A robot is a strange kind of listener: not fully predictable like a person, not fully mechanical like a button. That uncertainty is exactly what makes it useful for studying calibration. People had to decide, in real time, how much to explain, with no script to fall back on.</p>
</div>

<div class="case-block">
  <div class="case-block-label">What I built to measure it</div>
  <p>Before I could test anything, I needed a way to measure detail level precisely, not just sentence length. I built a custom metric, <strong>semantic detail density</strong>: the number of distinct, meaning-relevant pieces of information a person packed into a single response.</p>
</div>

<div class="case-step">
  <div class="case-step-number">1</div>
  <div class="case-step-body">
    <h3 class="case-step-title">Does the listener change what people say?</h3>
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
    <h3 class="case-step-title">Which signals actually change behavior?</h3>
    <p>I tested two signals from the robot together instead of one at a time: whether it opened by claiming competence, and whether it gave specific praise on a correct guess.</p>
    <div class="case-result">
      <span class="case-result-label">Result</span>
      Neither signal, nor the combination, moved the metric. But a signal we hadn't tested as a primary hypothesis did: when the robot explicitly said it failed and asked for another try, people immediately added more detail on the next response, then reverted back to baseline right after.
    </div>
  </div>
</div>

<div class="case-insight">
  <div class="case-insight-label">The pattern underneath both results</div>
  <p>Vague positive signals don't change behavior. Specific, actionable ones do. Telling someone something worked, or that the system is capable, doesn't reliably shift what they do next. Telling them precisely what didn't work, at a moment they can still act on it, does, immediately and measurably.</p>
</div>

<div class="pub-actions">
  <a class="pub-btn pub-doi" href="/academia/">Full write-ups &amp; citations</a>
</div>

**Tools:** R, custom behavioral coding, reproducible analysis
