---
title: Talking to Robots
permalink: /projects/talking-to-robots/
layout: page
excerpt: Two controlled experiments on how people talk to machines — reframed as an A/B test and a multivariate test.
comments: false
---
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,400;0,9..144,800;1,9..144,500&family=DM+Mono:wght@400;500&family=Instrument+Sans:wght@400;600&display=swap" rel="stylesheet">
<style>
/* ===== Talking to Robots: scoped styles (everything lives under .ttr) ===== */
.ttr{--paper:#f3ede2;--ink:#14213d;--pop:#ff5a1f;--mint:#2ec4b6;--card:#fffaf0;--muted:#5d6477;--line:#14213d22;
  background:var(--paper);color:var(--ink);font:18px/1.6 "Instrument Sans",system-ui,sans-serif;border-radius:28px;padding:8px 26px 40px;margin:0 auto;overflow:hidden}
@media (prefers-color-scheme:dark){.ttr{--paper:#0f1424;--ink:#f3ede2;--pop:#ff7a45;--mint:#41d6c8;--card:#171e36;--muted:#9aa3bd;--line:#f3ede233}}
/* If your theme toggles dark mode with an attribute or class, these follow it. Adjust to match. */
html[data-theme="dark"] .ttr,html[data-mode="dark"] .ttr,html.dark .ttr,body.dark .ttr{--paper:#0f1424;--ink:#f3ede2;--pop:#ff7a45;--mint:#41d6c8;--card:#171e36;--muted:#9aa3bd;--line:#f3ede233}
html[data-theme="light"] .ttr,html[data-mode="light"] .ttr{--paper:#f3ede2;--ink:#14213d;--pop:#ff5a1f;--mint:#2ec4b6;--card:#fffaf0;--muted:#5d6477;--line:#14213d22}
.ttr *{box-sizing:border-box}
.ttr .mono,.ttr .pub-meta,.ttr .case-block-label,.ttr .case-result-label,.ttr .case-insight-label{font-family:"DM Mono",ui-monospace,monospace;font-size:12px;letter-spacing:.14em;text-transform:uppercase}
.ttr p{margin:0 0 14px;max-width:640px}
.ttr a{color:inherit}
main > h1:first-of-type,article > header > h1,.page-title{display:none}

/* hero */
.ttr-hero{position:relative;padding:34px 0 8px}
.ttr .pub-meta{color:var(--pop);margin:0 0 6px;max-width:none}
.ttr h1{font:800 clamp(54px,12vw,128px)/.9 Fraunces,Georgia,serif;letter-spacing:-.04em;margin:14px 0 18px;color:var(--ink)}
.ttr h1 em{font-style:italic;font-weight:500;color:var(--pop)}
.ttr-robot{position:absolute;right:0;top:20px;width:min(24vw,140px);color:var(--ink)}
.ttr-stamp{display:inline-flex;gap:10px;align-items:center;border:2px solid var(--ink);border-radius:99px;padding:8px 16px;transform:rotate(-2deg);background:var(--mint);color:#07261f;font:500 14px "DM Mono",monospace}

/* tags as a ticker */
.ttr .pub-tags{border-block:2px solid var(--ink);margin:30px -26px 0;overflow:hidden;white-space:nowrap;background:var(--ink)}
.ttr .pub-tags-track{display:inline-block;padding:10px 0;animation:ttr-m 24s linear infinite}
.ttr .pub-tag{display:inline-block;margin:0 26px;color:var(--paper);font:500 13px "DM Mono",monospace;letter-spacing:.08em;text-transform:uppercase;background:none;border:0;padding:0}
.ttr .pub-tag::after{content:"✦";margin-left:52px;color:var(--pop)}
@keyframes ttr-m{to{transform:translateX(-50%)}}

/* short version */
.ttr-short{margin:40px 0 0;display:grid;gap:14px}
.ttr-short .mono{color:var(--muted)}
.ttr-a{display:grid;grid-template-columns:56px 1fr;gap:14px;align-items:start;background:var(--card);border:2px solid var(--ink);border-radius:18px;padding:16px 20px;box-shadow:6px 6px 0 var(--ink)}
.ttr-a i{font:800 42px/1 Fraunces,serif;font-style:normal;color:var(--pop)}
.ttr-a:nth-of-type(2) i{color:var(--mint)}

/* case blocks = chapters */
.ttr .case-block{position:relative;padding:54px 0 0;counter-increment:ttrc}
.ttr{counter-reset:ttrc}
.ttr .case-block::before{content:counter(ttrc);position:absolute;right:0;top:34px;font:800 clamp(90px,18vw,160px)/.8 Fraunces,serif;color:transparent;-webkit-text-stroke:2px var(--ink);opacity:.16;pointer-events:none}
.ttr .case-block-label{color:var(--pop);position:relative;margin-bottom:10px}
.ttr .case-block p{position:relative;font:500 clamp(20px,2.8vw,26px)/1.4 Fraunces,serif}
.ttr .case-block em{font-style:italic;color:var(--pop)}
.ttr .case-block strong{background:linear-gradient(transparent 62%,var(--mint) 62%)}

/* task widget */
.ttr-game{display:grid;grid-template-columns:1fr;gap:14px;margin:22px 0 4px}
@media(min-width:720px){.ttr-game{grid-template-columns:1fr 1.2fr 1fr}}
.ttr-tile{background:var(--card);border:2px solid var(--ink);border-radius:18px;padding:16px;text-align:center}
.ttr-tile .mono{color:var(--muted);font-size:11px}
.ttr-word{font:800 36px Fraunces,serif;margin-top:12px;filter:blur(7px);transition:filter .3s;user-select:none}
.ttr-word.on{filter:none}
.ttr-ring{position:relative;width:124px;height:124px;margin:8px auto 0}
.ttr-ring svg{transform:rotate(-90deg)}
.ttr-ring circle{fill:none;stroke-width:10}
.ttr-ring .bg{stroke:var(--line)}
.ttr-ring .fg{stroke:var(--pop);stroke-linecap:round;stroke-dasharray:339.3;stroke-dashoffset:0}
.ttr-ring b{position:absolute;inset:0;display:grid;place-items:center;font:800 38px Fraunces,serif}
.ttr-go{margin-top:10px;font:600 15px "Instrument Sans",sans-serif;border:2px solid var(--ink);background:var(--pop);color:#fff;border-radius:99px;padding:7px 16px;cursor:pointer;box-shadow:3px 3px 0 var(--ink)}
.ttr-go:active{transform:translate(2px,2px);box-shadow:1px 1px 0 var(--ink)}
.ttr-who{display:flex;gap:10px;justify-content:center;font-size:34px;margin:12px 0 6px}
.ttr-who span{opacity:.3;transition:.2s}
.ttr-who span.on{opacity:1;transform:scale(1.15)}
.ttr-fine{font:12px/1.5 "DM Mono",monospace;color:var(--muted);max-width:640px}

/* metric widget */
.ttr-metric{background:var(--ink);color:var(--paper);border-radius:22px;padding:26px 24px;margin:20px 0 0}
.ttr-metric .mono{color:var(--mint)}
.ttr-say{font:500 clamp(22px,3.6vw,32px)/1.5 Fraunces,serif;margin:12px 0 16px}
.ttr-say button{font:inherit;color:inherit;background:none;border:0;border-bottom:3px dashed var(--muted);padding:0 2px;cursor:pointer;transition:.2s}
.ttr-say button.on{background:var(--pop);border-color:var(--pop);color:#fff;border-radius:6px}
.ttr-meter{display:flex;align-items:center;gap:14px}
.ttr-score{font:800 60px/1 Fraunces,serif;color:var(--mint);min-width:40px}

/* study steps */
.ttr .case-step{display:flex;margin:34px 0;border:2px solid var(--ink);border-radius:26px;background:var(--card);overflow:hidden;box-shadow:8px 8px 0 var(--ink)}
.ttr .case-step-number{flex:0 0 64px;display:grid;place-items:start center;padding-top:18px;background:var(--pop);color:#fff;border-right:2px solid var(--ink);font:800 38px/1 Fraunces,serif}
.ttr .case-step:nth-of-type(2) .case-step-number{background:var(--mint);color:#07261f}
.ttr .case-step-body{padding:24px 24px 26px;min-width:0}
.ttr .case-step-title{font:800 clamp(24px,3.6vw,34px)/1.12 Fraunces,serif;letter-spacing:-.015em;margin:0 0 14px}
.ttr .case-result{background:var(--paper);border:2px solid var(--ink);border-radius:16px;padding:16px 18px;margin:20px 0 0;max-width:660px}
.ttr .case-result-label{display:block;background:var(--ink);color:var(--paper);width:max-content;border-radius:99px;padding:3px 12px;margin-bottom:10px;font-size:11px}

/* study 1 compare */
.ttr .vs-compare{display:flex;align-items:center;gap:12px;flex-wrap:wrap;margin:18px 0 6px}
.ttr .vs-chip{border:2px solid var(--ink);border-radius:99px;padding:6px 16px;font:600 15px "Instrument Sans",sans-serif;background:var(--paper)}
.ttr .vs-chip:first-child{background:var(--mint);color:#07261f}
.ttr .vs-chip:last-child{background:var(--pop);color:#fff}
.ttr .vs-versus{font:italic 500 20px Fraunces,serif;color:var(--muted)}
.ttr-bars{display:grid;gap:10px;margin:12px 0 6px;max-width:560px}
.ttr-bars .row{display:grid;grid-template-columns:96px 1fr;gap:12px;align-items:center}
.ttr-bars .track{height:34px;border-radius:99px;border:2px solid var(--ink);position:relative;overflow:hidden;background:var(--paper)}
.ttr-bars .track i{position:absolute;inset:0 auto 0 0;width:0;transition:width 1.1s cubic-bezier(.2,.8,.2,1)}
.ttr-bars .h i{background:var(--mint)} .ttr-bars .r i{background:var(--pop)}
.ttr-bars.in-view .h i{width:38%} .ttr-bars.in-view .r i{width:84%}

/* study 2 matrix */
.ttr .matrix-2x2{display:grid;grid-template-columns:110px 1fr 1fr;gap:8px;margin:20px 0 6px;max-width:560px}
.ttr .matrix-cell{border:2px solid var(--ink);border-radius:14px;padding:14px 8px;text-align:center;background:var(--paper);font-size:15px}
.ttr .matrix-corner{border:0;background:none}
.ttr .matrix-head{border:0;background:none;font:500 11px "DM Mono",monospace;letter-spacing:.1em;text-transform:uppercase;color:var(--muted);display:flex;align-items:center;justify-content:center;padding:6px}
.ttr .matrix-cell:not(.matrix-head):not(.matrix-corner)::before{content:"";display:block;width:44px;height:3px;border-radius:3px;background:var(--ink);margin:0 auto 8px}
.ttr .matrix-caption{font:12px/1.5 "DM Mono",monospace;color:var(--muted);margin-top:8px}
.ttr-zig{margin:6px 0 0;max-width:660px}
.ttr-zig svg{width:100%;height:auto;display:block;background:var(--ink);border-radius:16px;padding:10px}
.ttr-zig .base{stroke:#9aa3bd;stroke-width:2;stroke-dasharray:4 6;fill:none}
.ttr-zig .ln{stroke:var(--mint);stroke-width:4;fill:none;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:700;stroke-dashoffset:700}
.ttr-zig.in-view .ln{animation:ttr-draw 1.8s .2s forwards}
@keyframes ttr-draw{to{stroke-dashoffset:0}}
.ttr-zig .dot{fill:var(--pop)}

/* takeaway */
.ttr .case-insight{margin:50px 0 10px;background:var(--pop);color:#fff;border:2px solid var(--ink);border-radius:30px;padding:36px 30px;box-shadow:10px 10px 0 var(--ink)}
.ttr .case-insight-label{opacity:.9;margin-bottom:12px}
.ttr .case-insight p{font:800 clamp(20px,2.9vw,28px)/1.25 Fraunces,serif;letter-spacing:-.01em;max-width:760px;margin:0}

/* action */
.ttr .pub-actions{margin:34px 0 6px}
.ttr .pub-btn{display:inline-block;text-decoration:none;font:600 16px "Instrument Sans",sans-serif;padding:14px 24px;border:2px solid var(--ink);border-radius:99px;background:var(--ink);color:var(--paper);box-shadow:4px 4px 0 var(--pop)}
.ttr .pub-btn:hover{transform:translate(-1px,-1px);box-shadow:6px 6px 0 var(--pop)}

@media(prefers-reduced-motion:reduce){.ttr .pub-tags-track,.ttr-zig.in-view .ln{animation:none}.ttr-zig .ln{stroke-dashoffset:0}.ttr-bars .track i{transition:none}}
@media(max-width:600px){.ttr{padding:4px 16px 30px}.ttr .pub-tags{margin-inline:-16px}.ttr-robot{display:none}.ttr-a{grid-template-columns:40px 1fr}.ttr .case-step-number{flex-basis:44px;font-size:28px}.ttr .case-step-body{padding:18px 16px}.ttr .matrix-2x2{grid-template-columns:76px 1fr 1fr}.ttr-bars .row{grid-template-columns:70px 1fr}}
</style>
<div class="ttr">
<div class="ttr-hero">
  <svg class="ttr-robot" viewBox="0 0 120 120" aria-hidden="true">
    <line x1="60" y1="6" x2="60" y2="22" stroke="currentColor" stroke-width="4" stroke-linecap="round"/>
    <circle cx="60" cy="8" r="6" fill="var(--pop)"/>
    <rect x="12" y="22" width="96" height="82" rx="26" fill="var(--card)" stroke="currentColor" stroke-width="4"/>
    <circle cx="42" cy="58" r="13" fill="var(--paper)" stroke="currentColor" stroke-width="3"/>
    <circle cx="78" cy="58" r="13" fill="var(--paper)" stroke="currentColor" stroke-width="3"/>
    <circle class="ttr-pupil" cx="42" cy="58" r="6" fill="currentColor"/>
    <circle class="ttr-pupil" cx="78" cy="58" r="6" fill="currentColor"/>
    <rect x="40" y="82" width="40" height="8" rx="4" fill="var(--pop)"/>
  </svg>
  <p class="pub-meta">PhD research on how people talk to machines &middot; Koç University &middot; 2020–2026</p>
  <h1>Talking to <em>Robots.</em></h1>
  <div class="ttr-stamp">★ HRI '26 · Honorable Mention</div>
</div>
<div class="pub-tags" aria-label="Skills">
  <div class="pub-tags-track">
    <span class="pub-tag">A/B Testing</span>
    <span class="pub-tag">Multivariate Testing</span>
    <span class="pub-tag">Behavioral Analytics</span>
    <span class="pub-tag">R</span>
    <span class="pub-tag">Experimental Design</span>
    <span class="pub-tag" aria-hidden="true">A/B Testing</span>
    <span class="pub-tag" aria-hidden="true">Multivariate Testing</span>
    <span class="pub-tag" aria-hidden="true">Behavioral Analytics</span>
    <span class="pub-tag" aria-hidden="true">R</span>
    <span class="pub-tag" aria-hidden="true">Experimental Design</span>
  </div>
</div>
<div class="ttr-short">
  <div class="mono">The short version</div>
  <div class="ttr-a"><i>1</i><div>People gave a robot more detail than a human listener, every time, even after the robot got several answers right in a row.</div></div>
  <div class="ttr-a"><i>2</i><div>An upfront competence claim and specific positive feedback, alone or together, changed nothing.</div></div>
  <div class="ttr-a"><i>3</i><div>When the robot said it could not understand and asked for another description, people gave more detail for that one attempt only.</div></div>
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
  <div class="ttr-game">
    <div class="ttr-tile"><div class="mono">1 · The word</div><div class="ttr-word" id="ttr-word">truck</div></div>
    <div class="ttr-tile"><div class="mono">2 · Seven seconds</div>
      <div class="ttr-ring"><svg width="124" height="124" viewBox="0 0 132 132"><circle class="bg" cx="66" cy="66" r="54"/><circle class="fg" id="ttr-fg" cx="66" cy="66" r="54"/></svg><b id="ttr-t">7</b></div>
      <button class="ttr-go" id="ttr-go" type="button">▶ Play</button></div>
    <div class="ttr-tile"><div class="mono">3 · Who listens?</div>
      <div class="ttr-who" aria-hidden="true"><span id="ttr-p1">🧑</span><span id="ttr-p2">🤖</span></div>
      <div class="ttr-fine">Human or robot, same behavior.</div></div>
  </div>
</div>
<div class="case-block">
  <div class="case-block-label">📏 What I built to measure it</div>
  <p>Before I could test anything, I needed a way to measure the amount of content packed in people's word descriptions. So I built one: <strong>semantic detail density</strong>. It counts how many separate, meaningful pieces of information someone packs into what they say. Describing a truck as <em>"a large vehicle used to carry stuff"</em> scores three points of detail (large / vehicle / used for carrying).</p>
  <div class="ttr-metric">
    <div class="mono">Try it · tap each detail</div>
    <div class="ttr-say">“a <button type="button" data-d>large</button> <button type="button" data-d>vehicle</button> <button type="button" data-d>used to carry stuff</button>”</div>
    <div class="ttr-meter"><div class="ttr-score" id="ttr-score">0</div><div class="mono">points of detail</div></div>
  </div>
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
    <div class="ttr-bars" id="ttr-bars">
      <div class="row"><span class="mono">Human</span><div class="track h"><i></i></div></div>
      <div class="row"><span class="mono">Robot</span><div class="track r"><i></i></div></div>
    </div>
    <div class="ttr-fine">Schematic of the direction of the effect. Replace with your original figure.</div>
    <div class="case-result">
      <span class="case-result-label">Result</span>
      People gave the robot more detail than the human, every time. They kept doing this even after the robot got several answers right in a row. Doing well was not enough to make people explain less. This was published as a short paper at ACM/IEEE HRI '26 and won an Honorable Mention award.
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
    <div class="ttr-zig" id="ttr-zig" style="margin-top:16px">
      <svg viewBox="0 0 600 150" role="img" aria-label="Schematic: detail rises on the retry attempt, then returns to baseline">
        <path class="base" d="M20 110H580"/>
        <path class="ln" d="M20 110H190L260 30L330 110H580"/>
        <circle class="dot" cx="260" cy="30" r="7"/>
        <text x="275" y="30" fill="#f3ede2" font-family="DM Mono,monospace" font-size="13">retry attempt</text>
        <text x="20" y="140" fill="#9aa3bd" font-family="DM Mono,monospace" font-size="12">baseline</text>
      </svg>
      <div class="ttr-fine" style="margin-top:6px">Schematic. Replace with your actual data.</div>
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
</div>
<script>
(function(){
  var root=document.querySelector('.ttr'); if(!root) return;
  var pupils=[].slice.call(root.querySelectorAll('.ttr-pupil')), robot=root.querySelector('.ttr-robot');
  addEventListener('pointermove',function(e){
    var bb=robot.getBoundingClientRect(); if(!bb.width) return;
    var a=Math.atan2(e.clientY-(bb.top+bb.height/2),e.clientX-(bb.left+bb.width/2));
    pupils.forEach(function(p){p.style.transform='translate('+Math.cos(a)*5+'px,'+Math.sin(a)*5+'px)'});
  });
  var go=document.getElementById('ttr-go'),fg=document.getElementById('ttr-fg'),t=document.getElementById('ttr-t'),w=document.getElementById('ttr-word'),
      p1=document.getElementById('ttr-p1'),p2=document.getElementById('ttr-p2'),run=false,who=1;
  go.addEventListener('click',function(){
    if(run) return; run=true; who^=1; w.classList.add('on');
    p1.classList.toggle('on',who===0); p2.classList.toggle('on',who===1);
    var s=Date.now(),L=339.3,iv=setInterval(function(){
      var e=(Date.now()-s)/1000,left=Math.max(0,7-e);
      fg.style.strokeDashoffset=L*(e/7); t.textContent=Math.ceil(left);
      if(left<=0){clearInterval(iv);run=false;w.classList.remove('on');t.textContent='7';fg.style.strokeDashoffset=0;go.textContent='▶ Play again'}
    },50);
  });
  var sc=document.getElementById('ttr-score');
  [].forEach.call(root.querySelectorAll('[data-d]'),function(el){
    el.addEventListener('click',function(){el.classList.toggle('on');sc.textContent=root.querySelectorAll('[data-d].on').length});
  });
  var targets=[document.getElementById('ttr-bars'),document.getElementById('ttr-zig')];
  if('IntersectionObserver' in window){
    var io=new IntersectionObserver(function(es){es.forEach(function(e){if(e.isIntersecting){e.target.classList.add('in-view');io.unobserve(e.target)}})},{threshold:.4});
    targets.forEach(function(el){io.observe(el)});
  } else { targets.forEach(function(el){el.classList.add('in-view')}); }
})();
</script>
