---
title: About
permalink: /about/
layout: page
excerpt: Behavioral researcher with a recent PhD in Psychology (Cognitive Track) from Koç University, moving that experimental mindset into product and research work.
comments: false
---
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<style>
/* About page. Every rule is scoped to .abt and every class is prefixed abt-, so nothing here touches the rest of the site. Look: a bento grid of tiles, one font (Plus Jakarta Sans), one accent (lime). */
.header:has(+ .page-content .abt){display:none}
.abt{--bg:#efeee9;--tile:#fff;--ink:#121316;--muted:#6a6d75;--line:rgba(18,19,22,.1);--acc:#d4f15a;--on-acc:#121316;--deep:#121316;--on-deep:#f3f2ec;
  background:var(--bg);color:var(--ink);font-family:"Plus Jakarta Sans",system-ui,-apple-system,"Segoe UI",Roboto,sans-serif;font-size:17px;line-height:1.6;text-align:left;max-width:980px;margin:0 auto;padding:18px;border-radius:26px}
body[data-theme="dark"] .abt{--bg:#0f1013;--tile:#1a1b20;--ink:#f1f0ea;--muted:#9b9ea7;--line:rgba(241,240,234,.1);--deep:#f1f0ea;--on-deep:#121316}
.abt *,.abt *::before,.abt *::after{box-sizing:border-box}
.abt p{margin:0;padding:0;color:inherit;opacity:1}
.abt h1,.abt h2{font-family:inherit;color:inherit;margin:0;padding:0;border:0;text-transform:none;letter-spacing:normal}
.abt h2::before,.abt h2::after{content:none}
.abt a{color:inherit}
.abt a::after{content:none!important}
.abt b,.abt strong{color:inherit!important}
.abt em,.abt i{font-style:normal}
.abt ol,.abt ul{list-style:none!important;margin:0;padding:0}
.abt li{list-style:none!important}
.abt li::before{content:none}

.abt-grid{display:grid;grid-template-columns:repeat(6,1fr);gap:14px}
.abt-t{background:var(--tile);border-radius:22px;padding:26px;position:relative;overflow:hidden;opacity:0;transform:translateY(14px);transition:opacity .6s,transform .6s cubic-bezier(.2,.8,.2,1)}
.abt-t.on{opacity:1;transform:none}
.abt-k{display:block;font-size:12.5px;font-weight:700;letter-spacing:.08em;text-transform:uppercase;color:var(--muted);margin-bottom:14px}

.abt-intro{grid-column:span 4;grid-row:span 2;padding:34px 34px 30px;display:flex;flex-direction:column}
.abt p.abt-name{font-weight:700;font-size:15px;color:var(--muted);margin-bottom:26px}
.abt h1.abt-h1{font-weight:800;font-size:clamp(36px,5.6vw,58px);line-height:1.05;letter-spacing:-.035em;margin-bottom:24px}
.abt-h1 span{display:inline;background:linear-gradient(transparent 58%,var(--acc) 58%);padding:0 .06em}
body[data-theme="dark"] .abt-h1 span{background:none;color:var(--acc)}
.abt p.abt-lead{font-size:17.5px;line-height:1.65;color:var(--ink);max-width:560px;margin-top:auto}

.abt-phd{grid-column:span 2;background:var(--acc);color:var(--on-acc)}
.abt-phd .abt-k{color:var(--on-acc);opacity:.65}
.abt-phd b{display:block;font-weight:800;font-size:26px;line-height:1.15;letter-spacing:-.02em;margin-bottom:10px}
.abt-phd p{font-weight:600;font-size:15px;line-height:1.5}

.abt-open{grid-column:span 2;background:var(--deep);color:var(--on-deep);display:flex;flex-direction:column;justify-content:space-between;gap:18px}
.abt-open .abt-k{color:var(--on-deep);opacity:.6;margin:0}
.abt-open b{display:flex;align-items:center;gap:12px;font-weight:800;font-size:21px;line-height:1.25;letter-spacing:-.015em}
.abt-open b i{flex:0 0 12px;height:12px;border-radius:50%;background:var(--acc);animation:abt-pulse 2s infinite}
body[data-theme="dark"] .abt-open b i{background:#6e8f00}
@keyframes abt-pulse{0%{box-shadow:0 0 0 0 rgba(212,241,90,.5)}70%{box-shadow:0 0 0 12px rgba(212,241,90,0)}100%{box-shadow:0 0 0 0 rgba(212,241,90,0)}}

.abt-path{grid-column:span 6;padding:30px 30px 28px}
.abt-steps{display:grid;grid-template-columns:repeat(4,1fr);gap:18px;position:relative;margin-top:6px}
.abt-steps::before{content:"";position:absolute;left:8px;right:8px;top:8px;height:2px;background:var(--line)}
.abt-steps::after{content:"";position:absolute;left:8px;top:8px;height:2px;width:0;background:var(--ink);transition:width 1.4s ease-out .2s}
.abt-path.on .abt-steps::after{width:calc(100% - 16px)}
.abt-steps li{position:relative;padding-top:34px!important;margin:0!important}
.abt-steps li::after{content:"";position:absolute;left:0;top:0;width:18px;height:18px;border-radius:50%;background:var(--tile);border:2px solid var(--ink);transition:background .3s .6s}
.abt-path.on .abt-steps li::after{background:var(--ink)}
.abt-steps li.hl::after{background:var(--acc)!important;border-color:var(--ink);box-shadow:0 0 0 4px var(--acc)}
.abt-steps b{display:block;font-weight:800;font-size:17.5px;line-height:1.25;letter-spacing:-.01em;margin-bottom:6px}
.abt-steps span{display:block;font-size:14.5px;line-height:1.5;color:var(--muted)}
.abt-steps em{display:inline-block;margin-top:10px;font-weight:700;font-size:13px;line-height:1.35;background:var(--acc);color:var(--on-acc);border-radius:8px;padding:4px 9px}
.abt .abt-steps a{color:var(--ink)!important;text-decoration:underline;text-underline-offset:3px}

.abt-skill{grid-column:span 3}
.abt-skill svg{width:38px;height:38px;display:block;margin-bottom:16px;stroke:var(--ink);fill:none;stroke-width:2.2;stroke-linecap:round;stroke-linejoin:round;transition:transform .25s}
.abt-skill svg .a{fill:var(--acc)}
.abt-skill h2{font-weight:800;font-size:22px;letter-spacing:-.02em;margin-bottom:8px}
.abt-skill p{font-size:15.5px;line-height:1.6;color:var(--muted)}
.abt-skill:hover svg{transform:rotate(-6deg) scale(1.06)}

.abt-next{grid-column:span 4;background:var(--deep);color:var(--on-deep);padding:32px 34px}
.abt-next .abt-k{color:var(--on-deep);opacity:.6}
.abt-next p{font-weight:700;font-size:clamp(20px,2.5vw,25px);line-height:1.4;letter-spacing:-.015em}
.abt-next p mark{background:var(--acc);color:var(--on-acc);border-radius:6px;padding:0 .2em;box-decoration-break:clone;-webkit-box-decoration-break:clone}

.abt-go{grid-column:span 2;display:flex;flex-direction:column;gap:10px;padding:22px}
.abt a.abt-btn,.abt a.abt-btn:visited{color:var(--ink)!important}
.abt a.abt-btn:hover{color:var(--on-acc)!important}
.abt a.abt-btn{display:flex;align-items:center;justify-content:space-between;text-decoration:none;font-weight:700;font-size:17px;padding:15px 16px;border-radius:14px;background:var(--bg);transition:background .2s,transform .2s,color .2s}
.abt a.abt-btn i{font-weight:800;transition:transform .2s}
.abt a.abt-btn:hover{background:var(--acc);color:var(--on-acc);transform:translateY(-2px)}
.abt a.abt-btn:hover i{transform:translateX(4px)}

@media(max-width:820px){.abt-intro,.abt-path,.abt-next,.abt-go{grid-column:span 6}.abt-phd,.abt-open,.abt-skill{grid-column:span 3}.abt-intro{grid-row:auto}}
@media(max-width:600px){.abt{padding:10px;border-radius:18px;font-size:16px}.abt-grid{gap:10px}.abt-grid>*{grid-column:span 6!important}.abt-t{padding:22px}.abt-intro{padding:26px 22px}.abt .abt-steps{grid-template-columns:1fr;gap:20px;padding-left:34px}.abt-steps::before{left:8px;right:auto;top:8px;bottom:8px;width:2px;height:auto}.abt-steps::after{left:8px;top:8px;width:2px!important;height:0;transition:height 1.4s ease-out .2s}.abt-path.on .abt-steps::after{height:calc(100% - 16px)}.abt-steps li{padding-top:0!important}.abt-steps li::after{left:-34px}}
@media(prefers-reduced-motion:reduce){.abt *{animation:none!important;transition:none!important}.abt-t{opacity:1;transform:none}}
</style>
<div class="abt">
<div class="abt-grid">
  <div class="abt-t abt-intro">
    <p class="abt-name">Hande Sodacı, PhD · UX &amp; behavioral researcher</p>
    <h1 class="abt-h1">People talk differently to robots. <span>I study how.</span></h1>
    <p class="abt-lead">I am a user experience and behavioral researcher with a PhD in Psychology from Koç University (2020–2026) and extensive experience designing controlled experiments and making sense of real behavioral data. My work looks at how people change the way they communicate — what they say, when, and how much detail they give — when talking to a robot or another conversational agent instead of another person.</p>
  </div>
  <div class="abt-t abt-phd">
    <span class="abt-k">Degree</span>
    <b>PhD in Psychology</b>
    <p>Cognitive Track · Koç University · 2020–2026</p>
  </div>
  <div class="abt-t abt-open">
    <span class="abt-k">Now</span>
    <b><i></i>Open to product and research roles</b>
  </div>
  <div class="abt-t abt-path">
    <span class="abt-k">Background</span>
    <ol class="abt-steps">
      <li><b>Boğaziçi University</b><span>BA in Psychology, with a certificate in Linguistics</span></li>
      <li><b>Radboud University</b><span>Research master's in Language and Communication, the Netherlands</span></li>
      <li class="hl"><b>Tilburg University</b><span>Research assistant on the EU Horizon 2020 <a href="/academia/">L2TOR</a> project, designing a personalized language-learning study for bilingual children using a social robot</span><em>Where my interest in human–robot interaction started</em></li>
      <li><b>Koç University</b><span>PhD in Psychology. In the earlier years, I also coordinated a TÜBİTAK-funded longitudinal study at MEF University.</span></li>
    </ol>
  </div>
  <div class="abt-t abt-skill">
    <svg viewBox="0 0 40 40" aria-hidden="true"><path d="M15 5h10M17 5v10L8 31a3 3 0 0 0 2.6 4.5h18.8A3 3 0 0 0 32 31l-9-16V5"/><path class="a" d="M11.5 25h17l3 6a2 2 0 0 1-1.8 3H10.3a2 2 0 0 1-1.8-3Z"/></svg>
    <h2>Testing</h2>
    <p>I design and run controlled experiments. My dissertation work covers 200+ participants and thousands of individual responses.</p>
  </div>
  <div class="abt-t abt-skill">
    <svg viewBox="0 0 40 40" aria-hidden="true"><path d="M5 35h30M5 35V5"/><rect class="a" x="10" y="20" width="6" height="11" rx="1.5"/><rect x="19" y="13" width="6" height="18" rx="1.5"/><rect class="a" x="28" y="8" width="6" height="23" rx="1.5"/></svg>
    <h2>Analyzing</h2>
    <p>I use statistical modeling in R to find real, sometimes subtle, patterns in how people behave, including when a result does not turn out the way I expected.</p>
  </div>
  <div class="abt-t abt-skill">
    <svg viewBox="0 0 40 40" aria-hidden="true"><rect class="a" x="8" y="12" width="24" height="19" rx="7"/><path d="M20 12V6"/><circle cx="20" cy="5" r="1.6"/><circle cx="15" cy="21" r="2"/><circle cx="25" cy="21" r="2"/><path d="M16 27h8"/></svg>
    <h2>Building</h2>
    <p>I build the technical side of these studies, including programming robot interactions. I also hold an Associate Degree in Web Design and Coding from Anadolu University, and I set up and customized this site myself.</p>
  </div>
  <div class="abt-t abt-skill">
    <svg viewBox="0 0 40 40" aria-hidden="true"><path class="a" d="M6 8h20a3 3 0 0 1 3 3v11a3 3 0 0 1-3 3H15l-7 6v-6H6a3 3 0 0 1-3-3V11a3 3 0 0 1 3-3Z"/><path d="M29 14h5a3 3 0 0 1 3 3v9a3 3 0 0 1-3 3h-1v5l-6-5h-5"/></svg>
    <h2>Communicating</h2>
    <p>I write up findings for both academic and general audiences, and produce research posters, slide decks, and presentations, judging whether a piece of content or design actually lands, rather than assuming it does.</p>
  </div>
  <div class="abt-t abt-next">
    <span class="abt-k">Where I am headed</span>
    <p>I am moving that experimental mindset into product and research roles — work that tests how people actually behave and turns that into something useful, <mark>at a faster pace than academic research allows.</mark></p>
  </div>
  <div class="abt-t abt-go">
    <a class="abt-btn" href="/projects/talking-to-robots/">My projects<i aria-hidden="true">→</i></a>
    <a class="abt-btn" href="/assets/HS_resume_202611.pdf">Resume (PDF)<i aria-hidden="true">→</i></a>
    <a class="abt-btn" href="/contact/">Get in touch<i aria-hidden="true">→</i></a>
  </div>
</div>
</div>
<script>
(function () {
  var root = document.querySelector(".abt");
  if (!root) { return; }
  var tiles = [].slice.call(root.querySelectorAll(".abt-t"));
  if (!("IntersectionObserver" in window) || matchMedia("(prefers-reduced-motion: reduce)").matches) {
    tiles.forEach(function (t) { t.classList.add("on"); });
    return;
  }
  var io = new IntersectionObserver(function (es) {
    es.forEach(function (e) {
      if (e.isIntersecting) {
        var t = e.target;
        setTimeout(function () { t.classList.add("on"); }, (tiles.indexOf(t) % 4) * 90);
        io.unobserve(t);
      }
    });
  }, { threshold: 0.15 });
  tiles.forEach(function (t) { io.observe(t); });
})();
</script>
