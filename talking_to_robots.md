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

<div class="case-block">
  <div class="case-block-label">The problem</div>
  <p>How much should a conversational agent (a robot, a chatbot, a voice assistant) signal what it understands to the person using it? Too little, and people may give it more information than it needs. Too much, and the signal may not change their behavior at all. My research tested how people adjust the amount of detail they give a conversational agent based on the signals it sends about whether it understood them.</p>
</div>

<div class="case-block">
  <div class="case-block-label">Why this was a useful test environment</div>
  <p>A robot is a strange kind of listener — not predictable like a person, not mechanical like a button. People cannot rely on their usual social shortcuts to guess what it understands, so it becomes a clean setting for isolating which signals people actually rely on, versus which ones they just assume should matter.</p>
</div>

<div class="case-block">
  <div class="case-block-label">What I built to measure it</div>
  <p>Before testing anything, I needed a sharper way to measure detail than sentence length could offer. So I built one: <strong>semantic detail density</strong>, a custom metric counting the distinct, meaning-relevant pieces of information packed into a single response. Describing a truck as <em>"a large vehicle used to carry stuff"</em> scores three points of detail.</p>
</div>

<div class="case-step">
  <div class="case-step-number">1</div>
  <div class="case-step-body">
    <h3 class="case-step-title">Does the listener change what people say?</h3>
    <p>Participants described words to a human listener or a robot listener — same timing, same accuracy, same errors, down to the second. The only thing that changed was who was listening.</p>
    <div class="vs-compare">
      <span class="vs-chip">Human listener</span>
      <span class="vs-versus">vs</span>
      <span class="vs-chip">Robot listener</span>
    </div>
    <div class="case-result">
      <span class="case-result-label">Result</span>
      People gave the robot more detail than the human, every time, and never dialed it back, even after the robot nailed several answers in a row. Success alone was not enough to earn a shorter explanation. This became a published paper at ACM/IEEE HRI '26, and won an Honorable Mention.
    </div>
  </div>
</div>

<div class="case-step">
  <div class="case-step-number">2</div>
  <div class="case-step-body">
    <h3 class="case-step-title">Which signals actually change behavior?</h3>
    <p>Next, I tested two signals from the robot at once instead of one at a time: an upfront claim of competence, and specific positive feedback after a correct guess.</p>
    <div class="matrix-2x2">
      <div class="matrix-cell matrix-corner"></div>
      <div class="matrix-cell matrix-head">No competence claim</div>
      <div class="matrix-cell matrix-head">Competence claim</div>
      <div class="matrix-cell matrix-head">Generic feedback</div>
      <div class="matrix-cell">No effect</div>
      <div class="matrix-cell">No effect</div>
      <div class="matrix-cell matrix-head">Specific feedback</div>
      <div class="matrix-cell">No effect</div>
      <div class="matrix-cell">No effect</div>
    </div>
    <p class="matrix-caption">All four combinations tested — none moved the metric on their own.</p>
    <div class="case-result">
      <span class="case-result-label">Result</span>
      Neither moved the needle. Not the claim, not the feedback, not the combination. But one signal I had not even set out to test did: when the robot said flat out that it failed and asked for another try, people upped their detail instantly, then dropped straight back to baseline the moment after.
    </div>
  </div>
</div>

<div class="case-insight">
  <div class="case-insight-label">What this means in practice</div>
  <p>People did not change how much detail they gave just because the robot sounded confident or had been successful before. They changed when the robot gave a signal about what had just happened in that exact interaction. In other words, immediate and relevant feedback mattered more than general signs of competence.</p>
</div>

<div class="pub-actions">
  <a class="pub-btn pub-doi" href="/academia/">Full write-ups &amp; citations</a>
</div>

**Tools:** R, custom behavioral coding, reproducible analysis
