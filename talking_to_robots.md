---
title: Talking to Robots
permalink: /projects/talking-to-robots/
layout: page
excerpt: Two controlled experiments on how people talk to machines — reframed as an A/B test and a multivariate test.
comments: false
---

<p class="pub-meta">PhD research on how people talk to machines &middot; Koç University &middot; 2020–2026</p>

<div class="pub-tags">
  <span class="pub-tag">A/B Testing</span>
  <span class="pub-tag">Multivariate Testing</span>
  <span class="pub-tag">Behavioral Analytics</span>
  <span class="pub-tag">R</span>
  <span class="pub-tag">Experimental Design</span>
</div>

<div class="case-block">
  <div class="case-block-label">🤔 The problem</div>
  <p>How much should a robot, chatbot, or voice assistant tell someone it understands them? Too little, and people give it more than it needs. Too much, and it makes no difference at all. I tested how people change what they say based on the signals a system gives about whether it understood them.</p>
</div>

<div class="case-block">
  <div class="case-block-label">🎯 Why this was a useful test environment</div>
  <p>A robot is an odd kind of listener. It is not fully predictable like a person, and not fully simple like a button. People cannot use their normal social guesses to know what it understands. That makes it a clean way to see which signals actually change behavior, and which ones people just assume should matter.</p>
</div>

<div class="case-block">
  <div class="case-block-label">🎮 The task I built</div>
  <p>A game-based task: speakers saw a word and had seven seconds to describe it, without saying the word itself, while a human or a robot listener tried to guess it. Both listeners acted exactly the same way every time. So the only thing that ever changed was <em>who</em> was listening, not how they behaved.</p>
</div>

<div class="case-block">
  <div class="case-block-label">📏 What I built to measure it</div>
  <p>Before I could test anything, I needed a way to measure the amount of content packed in people's word descriptions. So I built one: <strong>semantic detail density</strong>. It counts how many separate, meaningful pieces of information someone packs into what they say. Describing a truck as <em>"a large vehicle used to carry stuff"</em> scores three points of detail (large / vehicle / used for carrying).</p>
</div>

<div class="case-step">
  <div class="case-step-number">1</div>
  <div class="case-step-body">
    <h3 class="case-step-title">Does the listener change what people say?</h3>
    <p>People described words to either a human listener or a robot listener. Everything else about the task stayed exactly the same.</p>
    <div class="vs-compare">
      <span class="vs-chip">Human listener</span>
      <span class="vs-versus">vs</span>
      <span class="vs-chip">Robot listener</span>
    </div>
    <div class="case-result">
      <span class="case-result-label">Result</span>
      People gave the robot more detail than the human, every time. They kept doing this even after the robot got several answers right in a row. Doing well was not enough to make people explain less. This became a published paper at ACM/IEEE HRI '26 and won an Honorable Mention.
    </div>
  </div>
</div>

<div class="case-step">
  <div class="case-step-number">2</div>
  <div class="case-step-body">
    <h3 class="case-step-title">Which signals actually change behavior?</h3>
    <p>Next, I tested two signals from the robot at the same time. First, the robot said upfront that it was good at understanding. Second, it gave specific positive feedback about how well the participant described the word, and correctly guessed it. On some rounds, the robot said it could not find the correct answer and asked for another description.</p>
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
      Neither the upfront competence claim nor the positive feedback changed anything, alone or together. But something interesting happened on the rounds when the robot said it could not understand and asked the participant to try again: people gave more detail right away as a response to this explicit call for help, but only for that one attempt. The moment after, they were back to normal.
    </div>
  </div>
</div>

<div class="case-insight">
  <div class="case-insight-label">💡 What this means in practice</div>
  <p>Looking at both results together, my read is this: people did not give more or less detail just because the robot sounded confident or had done well before. What actually moved them was the robot clearly saying it did not understand and asking to try again — a signal that was specific and something people could act on right then. In short, a clear, immediate signal mattered more than a general claim.</p>
</div>

<div class="pub-actions">
  <a class="pub-btn pub-doi" href="/academia/">Full write-ups &amp; citations</a>
</div>

**Tools:** R, custom behavioral coding, reproducible analysis
