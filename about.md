---
title: About
permalink: /about/
layout: page
excerpt: Behavioral researcher with a recent PhD in Psychology (Cognitive Track) from Koç University, moving that experimental mindset into product and research work.
comments: false
---
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Manrope:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<style>
/* About page. Every rule is scoped to .abt and every class is prefixed abt-, so nothing here touches the rest of the site. Look: minimalist, one font (Manrope), one accent color, lots of air. */
.header:has(+ .page-content .abt){display:none}
.abt{--bg:#fbfaf7;--ink:#16181d;--muted:#6b6f78;--line:rgba(22,24,29,.12);--acc:#ff5a36;--acc-soft:rgba(255,90,54,.12);
  background:var(--bg);color:var(--ink);font-family:"Manrope",system-ui,-apple-system,"Segoe UI",Roboto,sans-serif;font-size:18px;line-height:1.65;text-align:left;max-width:860px;margin:0 auto;padding:16px 32px 56px;border-radius:14px}
body[data-theme="dark"] .abt{--bg:#121318;--ink:#f1efe9;--muted:#9a9ea8;--line:rgba(241,239,233,.12);--acc:#ff7a59;--acc-soft:rgba(255,122,89,.14)}
.abt *,.abt *::before,.abt *::after{box-sizing:border-box}
.abt p{margin:0 0 14px;padding:0;color:inherit;opacity:1}
.abt h1,.abt h2{font-family:inherit;color:inherit;margin:0;padding:0;border:0;text-transform:none;letter-spacing:normal}
.abt h2::before,.abt h2::after{content:none}
.abt a{color:inherit}
.abt a::after{content:none!important}
.abt b,.abt strong{color:inherit}
.abt em,.abt i{font-style:normal}
.abt ol,.abt ul{list-style:none!important;margin:0;padding:0}
.abt li{list-style:none!important}
.abt li::before{content:none}

.abt-hero{padding:56px 0 20px}
.abt p.abt-name{font-weight:700;font-size:15px;letter-spacing:.02em;color:var(--muted);margin-bottom:22px}
.abt p.abt-name span{color:var(--acc);margin:0 6px}
.abt h1.abt-h1{font-weight:800;font-size:clamp(40px,7.4vw,76px);line-height:1.04;letter-spacing:-.035em;margin:0 0 30px;max-width:15ch}
.abt-rot{color:var(--acc);white-space:nowrap}
.abt-rot::after{content:"";display:inline-block;width:.06em;height:.82em;margin-left:.06em;vertical-align:-.06em;background:var(--acc);animation:abt-caret 1s steps(1) infinite}
@keyframes abt-caret{50%{opacity:0}}
.abt p.abt-lead{font-size:clamp(19px,2.3vw,22px);line-height:1.6;max-width:640px;color:var(--ink)}
.abt-status{display:inline-flex;align-items:center;gap:10px;margin-top:14px;font-weight:700;font-size:15px;padding:8px 16px;border:1.5px solid var(--line);border-radius:999px}
.abt-status i{width:9px;height:9px;border-radius:50%;background:var(--acc);box-shadow:0 0 0 0 var(--acc);animation:abt-pulse 2s infinite}
@keyframes abt-pulse{0%{box-shadow:0 0 0 0 var(--acc-soft)}70%{box-shadow:0 0 0 10px transparent}100%{box-shadow:0 0 0 0 transparent}}

.abt-sec{margin:72px 0 0;padding-top:22px;border-top:1.5px solid var(--line)}
.abt h2.abt-h2{display:flex;align-items:baseline;gap:14px;font-weight:800;font-size:clamp(26px,3.6vw,34px);letter-spacing:-.025em;margin-bottom:28px}
.abt-h2 span{font-size:14px;font-weight:700;color:var(--acc);letter-spacing:.04em}

.abt-path{position:relative;padding-left:34px!important}
.abt-path::before{content:"";position:absolute;left:7px;top:8px;bottom:8px;width:2px;background:var(--line)}
.abt-path::after{content:"";position:absolute;left:7px;top:8px;width:2px;height:var(--fill,0%);max-height:calc(100% - 16px);background:var(--acc);transition:height .6s ease-out}
.abt-path li{position:relative;padding:0 0 28px!important;margin:0!important;opacity:.25;transform:translateY(8px);transition:opacity .5s,transform .5s}
.abt-path li.on{opacity:1;transform:none}
.abt-path li::after{content:"";position:absolute;left:-33px;top:7px;width:16px;height:16px;border-radius:50%;background:var(--bg);border:2px solid var(--muted);transition:border-color .4s,background .4s}
.abt-path li.on::after{border-color:var(--acc);background:var(--acc)}
.abt-path li.next::after{background:var(--bg);border-style:dashed}
.abt-path b{display:block;font-weight:800;font-size:20px;letter-spacing:-.01em}
.abt-path span{display:block;color:var(--muted);font-size:16.5px;line-height:1.55;max-width:600px}
.abt-path em{display:inline-block;margin-top:8px;font-weight:700;font-size:14.5px;color:var(--acc);background:var(--acc-soft);border-radius:8px;padding:3px 10px}
.abt-path li.next b{color:var(--acc)}
.abt .abt-path a{color:var(--acc)!important;text-decoration:underline;text-underline-offset:3px}

.abt-do{display:grid;gap:0}
.abt-row{display:grid;grid-template-columns:200px 1fr;gap:24px;padding:22px 0;border-bottom:1.5px solid var(--line)}
.abt-row:first-child{padding-top:0}
.abt-row b{font-weight:800;font-size:22px;letter-spacing:-.015em}
.abt-row b small{display:block;font-size:52px;line-height:1;letter-spacing:-.04em;color:var(--acc);margin-bottom:6px}
.abt-row b small span{font-size:15px;letter-spacing:0;color:var(--muted);font-weight:700;display:block;margin-top:4px}
.abt-row p{margin:0;font-size:17px;color:var(--ink)}

.abt-next{font-weight:800;font-size:clamp(24px,3.6vw,36px);line-height:1.25;letter-spacing:-.025em;max-width:24ch}
.abt-next mark{background:linear-gradient(transparent 62%,var(--acc-soft) 62%);color:inherit;padding:0 .05em}

.abt-links{margin-top:30px;border-top:1.5px solid var(--line)}
.abt a.abt-link{display:flex;align-items:center;justify-content:space-between;gap:16px;text-decoration:none;padding:20px 0;border-bottom:1.5px solid var(--line);font-weight:800;font-size:clamp(20px,2.6vw,26px);letter-spacing:-.02em;transition:color .2s,padding .25s}
.abt a.abt-link span{font-weight:600;font-size:15px;color:var(--muted);letter-spacing:0;margin-left:auto}
.abt a.abt-link i{display:inline-grid;place-items:center;width:42px;height:42px;border-radius:50%;border:1.5px solid var(--line);font-weight:700;transition:transform .25s,background .2s,color .2s,border-color .2s}
.abt a.abt-link:hover{color:var(--acc);padding-left:8px}
.abt a.abt-link:hover i{transform:translateX(4px);background:var(--acc);border-color:var(--acc);color:#fff}

@media(max-width:640px){.abt{padding:8px 18px 40px;font-size:16px}.abt-hero{padding-top:36px}.abt-row{grid-template-columns:1fr;gap:8px}.abt a.abt-link span{display:none}.abt-sec{margin-top:56px}}
@media(prefers-reduced-motion:reduce){.abt *{animation:none!important;transition:none!important}.abt-path li{opacity:1;transform:none}}
</style>
<div class="abt">
<div class="abt-hero">
  <p class="abt-name">Hande Sodacı, PhD<span>/</span>UX &amp; behavioral researcher</p>
  <h1 class="abt-h1" aria-label="I study how people talk to robots and other conversational agents.">I study how people talk to <span class="abt-rot" id="abt-rot" aria-hidden="true">robots.</span></h1>
  <p class="abt-lead">I am a user experience and behavioral researcher with a PhD in Psychology from Koç University (2020–2026) and extensive experience designing controlled experiments and making sense of real behavioral data. My work looks at how people change the way they communicate — what they say, when, and how much detail they give — when talking to a robot or another conversational agent instead of another person.</p>
  <div class="abt-status"><i></i>Open to product and research roles</div>
</div>
<div class="abt-sec">
  <h2 class="abt-h2"><span>01</span>Background</h2>
  <ol class="abt-path" id="abt-path">
    <li><b>Boğaziçi University</b><span>BA in Psychology, with a certificate in Linguistics</span></li>
    <li><b>Radboud University, the Netherlands</b><span>Research master's in Language and Communication</span></li>
    <li><b>Tilburg University</b><span>Research assistant on the EU Horizon 2020 <a href="/academia/">L2TOR</a> project, designing a personalized language-learning study for bilingual children using a social robot.</span><em>Where my interest in human–robot interaction started</em></li>
    <li><b>Koç University</b><span>PhD in Psychology (Cognitive Track), 2020–2026. In the earlier years, I also coordinated a TÜBİTAK-funded longitudinal study at MEF University.</span></li>
    <li class="next"><b>Next: product and research roles</b><span>Work that tests how people actually behave.</span></li>
  </ol>
</div>
<div class="abt-sec">
  <h2 class="abt-h2"><span>02</span>What I actually do</h2>
  <div class="abt-do">
    <div class="abt-row"><b><small>200+</small>Experiments</b><p>I design and run controlled experiments. My dissertation work covers 200+ participants and thousands of individual responses.</p></div>
    <div class="abt-row"><b>Analysis</b><p>I use statistical modeling in R to find real, sometimes subtle, patterns in how people behave, including when a result does not turn out the way I expected.</p></div>
    <div class="abt-row"><b>Building</b><p>I build the technical side of these studies, including programming robot interactions. I also hold an Associate Degree in Web Design and Coding from Anadolu University, and I set up and customized this site myself.</p></div>
    <div class="abt-row"><b>Communicating</b><p>I write up findings for both academic and general audiences, and produce research posters, slide decks, and presentations, judging whether a piece of content or design actually lands, rather than assuming it does.</p></div>
  </div>
</div>
<div class="abt-sec">
  <h2 class="abt-h2"><span>03</span>Where I am headed</h2>
  <p class="abt-next">I am moving that experimental mindset into product and research roles: work that tests how people actually behave and turns that into something useful, <mark>at a faster pace than academic research allows.</mark></p>
  <div class="abt-links">
    <a class="abt-link" href="/projects/talking-to-robots/">See my projects<span>Research and past projects</span><i aria-hidden="true">→</i></a>
    <a class="abt-link" href="/assets/HS_resume_202611.pdf">Read my resume<span>Full background (PDF)</span><i aria-hidden="true">→</i></a>
    <a class="abt-link" href="/contact/">Get in touch<span>Contact form</span><i aria-hidden="true">→</i></a>
  </div>
</div>
</div>
<script>
(function () {
  var root = document.querySelector(".abt");
  if (!root) { return; }
  var reduce = matchMedia("(prefers-reduced-motion: reduce)").matches;

  var rot = document.getElementById("abt-rot");
  var words = ["robots.", "chatbots.", "voice assistants.", "other people."];
  var wi = 0;
  function erase(done) {
    var t = rot.textContent;
    if (!t.length) { done(); return; }
    rot.textContent = t.slice(0, -1);
    setTimeout(function () { erase(done); }, 45);
  }
  function type(w, done) {
    if (rot.textContent.length === w.length) { done(); return; }
    rot.textContent = w.slice(0, rot.textContent.length + 1);
    setTimeout(function () { type(w, done); }, 70);
  }
  function cycle() {
    setTimeout(function () {
      erase(function () {
        wi = (wi + 1) % words.length;
        type(words[wi], cycle);
      });
    }, 2200);
  }
  if (!reduce) { cycle(); }

  var path = document.getElementById("abt-path");
  var items = [].slice.call(path.querySelectorAll("li"));
  function fill() {
    var lit = items.filter(function (li) { return li.classList.contains("on"); });
    if (!lit.length) { return; }
    var last = lit[lit.length - 1];
    path.style.setProperty("--fill", (last.offsetTop + 15) + "px");
  }
  if ("IntersectionObserver" in window && !reduce) {
    var io = new IntersectionObserver(function (es) {
      es.forEach(function (e) {
        if (e.isIntersecting) { e.target.classList.add("on"); io.unobserve(e.target); fill(); }
      });
    }, { rootMargin: "0px 0px -20% 0px" });
    items.forEach(function (li) { io.observe(li); });
  } else {
    items.forEach(function (li) { li.classList.add("on"); });
    fill();
  }
})();
</script>
