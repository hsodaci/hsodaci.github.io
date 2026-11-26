---
title: About
permalink: /about/
layout: page
excerpt: Behavioral researcher with a recent PhD in Psychology (Cognitive Track) from Koç University, moving that experimental mindset into product and research work.
comments: false
---
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Archivo:wdth,wght@62..125,400..800&display=swap" rel="stylesheet">
<style>
/* About page, laid out as an academic research poster. Every rule is scoped to .abt and every class is prefixed abt-, so nothing here touches the rest of the site. One font family (Archivo), deep green and coral. */
.header:has(+ .page-content .abt){display:none}
.abt{--wall:#e9e6df;--sheet:#fffdf8;--ink:#1c2321;--muted:#5f6763;--line:rgba(28,35,33,.14);--grn:#0f5b4f;--on-grn:#f6f1e4;--acc:#ff7a59;--acc-soft:rgba(255,122,89,.22);--dim:rgba(28,35,33,.28);--fig:#eef3ef;
  font-family:"Archivo",system-ui,-apple-system,"Segoe UI",Roboto,sans-serif;font-stretch:100%;color:var(--ink);font-size:16.5px;line-height:1.58;text-align:left;
  max-width:1000px;margin:0 auto;padding:26px;background:var(--wall);border-radius:16px}
body[data-theme="dark"] .abt{--dim:rgba(236,235,229,.26);--wall:#0e1110;--sheet:#171c1a;--ink:#ecebe5;--muted:#a0a8a3;--line:rgba(236,235,229,.14);--grn:#1d7a6a;--fig:#202825}
.abt *,.abt *::before,.abt *::after{box-sizing:border-box}
.abt p{margin:0 0 12px;padding:0;color:inherit;opacity:1}
.abt h1,.abt h2,.abt h3{font-family:inherit;color:inherit;margin:0;padding:0;border:0;text-transform:none;letter-spacing:normal}
.abt h2::before,.abt h2::after,.abt h3::before,.abt h3::after{content:none}
.abt a{color:inherit}
.abt a::after{content:none!important}
.abt b,.abt strong{color:inherit!important}
.abt em,.abt i{font-style:normal}
.abt ol,.abt ul{list-style:none!important;margin:0;padding:0}
.abt li{list-style:none!important}
.abt li::before{content:none}
.abt table{border-collapse:collapse;width:100%;margin:0;border:0;display:table}
.abt tr,.abt th,.abt td{border:0!important;padding:0;background:none!important;text-align:left}
.abt .abt-bg tr:not(:last-child) td{border-bottom:1px solid var(--line)!important}
.abt .abt-refs a,.abt a.abt-more,.abt .abt-bg a{color:inherit!important}

.abt-sheet{position:relative;background:var(--sheet);border-radius:6px;box-shadow:0 1px 0 rgba(0,0,0,.04),0 18px 40px -18px rgba(0,0,0,.35);overflow:hidden}
.abt-sheet::before,.abt-sheet::after{content:"";position:absolute;top:10px;width:14px;height:14px;border-radius:50%;background:radial-gradient(circle at 35% 35%,#ff9e85,var(--acc) 60%,#c8452a);box-shadow:0 3px 4px rgba(0,0,0,.3);z-index:3}
.abt-sheet::before{left:12px}.abt-sheet::after{right:12px}

.abt-banner{background:var(--grn);color:var(--on-grn);padding:40px 44px 30px;display:grid;grid-template-columns:1fr auto;gap:24px;align-items:end}
.abt h1.abt-title{font-weight:800;font-stretch:112%;font-size:clamp(30px,4.6vw,50px);line-height:1.04;letter-spacing:-.02em;color:var(--on-grn);max-width:20ch}
.abt-title mark{background:none;color:var(--acc);padding:0}
.abt p.abt-authors{margin:16px 0 0;font-size:16px;font-weight:500;color:var(--on-grn);opacity:.9}
.abt-authors sup{font-size:.7em;color:var(--acc);font-weight:700}
.abt-ribbon{display:flex;flex-direction:column;align-items:flex-end;gap:10px}
.abt-ribbon span{white-space:nowrap;font-weight:700;font-size:13.5px;border-radius:999px;padding:6px 13px;background:rgba(255,255,255,.12);color:var(--on-grn)}
.abt-ribbon span.hot{background:var(--acc);color:#1c2321}
.abt-ribbon span.open::before{content:"";display:inline-block;width:8px;height:8px;border-radius:50%;background:#9ff0b9;margin-right:8px;animation:abt-pulse 2s infinite}
@keyframes abt-pulse{0%,100%{opacity:1}50%{opacity:.35}}

.abt-bar{display:flex;align-items:center;justify-content:space-between;gap:12px;padding:12px 44px;border-bottom:1.5px solid var(--line);font-size:14px;color:var(--muted);font-weight:600}
.abt-skim{font-family:inherit;font-weight:700;font-size:14px;border:1.5px solid var(--ink);background:none;color:var(--ink);border-radius:999px;padding:6px 14px;cursor:pointer;transition:background .2s,color .2s}
.abt-skim[aria-pressed="true"]{background:var(--acc);border-color:var(--acc);color:#1c2321}

.abt-cols{display:grid;grid-template-columns:1fr 1fr 1fr;gap:0}
.abt-col{padding:26px 26px 30px;border-right:1.5px solid var(--line)}
.abt-col:last-child{border-right:0}
.abt-sec{margin-bottom:26px}
.abt-sec:last-child{margin-bottom:0}
.abt h2.abt-h{display:flex;align-items:center;gap:10px;font-weight:800;font-stretch:108%;font-size:17px;letter-spacing:.01em;text-transform:uppercase;color:var(--on-grn);background:var(--grn);border-radius:4px;padding:6px 12px;margin-bottom:14px}
.abt-h span{display:grid;place-items:center;width:22px;height:22px;border-radius:50%;background:var(--on-grn);color:var(--grn);font-size:12.5px}

.abt-bg td{padding:9px 0;vertical-align:top}
.abt-bg td:first-child{width:76px;font-size:13px;font-weight:700;color:var(--muted);padding-top:11px}
.abt-bg b{display:block;font-weight:700;font-size:15.5px;line-height:1.3}
.abt-bg span{display:block;font-size:14px;line-height:1.45;color:var(--muted)}
.abt-bg tr.hl b{color:var(--grn)!important}
body[data-theme="dark"] .abt-bg tr.hl b{color:#7fd8c5!important}
.abt-bg em{display:inline-block;margin-top:5px;font-size:12.5px;font-weight:700;background:var(--acc-soft);border-radius:5px;padding:1px 7px}
.abt .abt-bg a{text-decoration:underline;text-underline-offset:2px}

.abt-m{padding:10px 0 12px;border-bottom:1px solid var(--line)}
.abt-m:last-child{border-bottom:0}
.abt-m h3{display:flex;align-items:center;gap:8px;font-weight:800;font-size:16.5px;margin-bottom:4px}
.abt-m h3::before{content:"";width:9px;height:9px;border-radius:2px;background:var(--acc);display:inline-block}
.abt-m p{font-size:14.5px;line-height:1.5;margin:0;color:var(--muted)}

.abt-res{margin-bottom:18px}
.abt-res p{font-size:15px}
.abt-fig{background:var(--fig);border-radius:6px;padding:12px 14px 10px;margin:4px 0 8px}
.abt-fig .row{display:grid;grid-template-columns:76px 1fr 38px;align-items:center;gap:8px;margin:5px 0;font-size:13px;font-weight:700}
.abt-fig .track{height:14px;background:rgba(0,0,0,.06);border-radius:3px;overflow:hidden}
body[data-theme="dark"] .abt-fig .track{background:rgba(255,255,255,.07)}
.abt-fig .track i{display:block;height:100%;width:0;background:var(--grn);border-radius:3px;transition:width 1s cubic-bezier(.2,.8,.2,1)}
.abt-fig .track i.a{background:var(--acc)}
.abt-fig.on .track i{width:var(--w)}
.abt-fig .row span:last-child{text-align:right;font-variant-numeric:tabular-nums}
.abt p.abt-cap{font-size:12.5px;line-height:1.4;color:var(--muted);margin:6px 0 0}
.abt-cap b{font-weight:800}
.abt a.abt-more{display:inline-block;font-weight:700;font-size:14px;text-decoration:none;border-bottom:2px solid var(--acc)}
.abt a.abt-more:hover{color:var(--acc)}

.abt-disc p{font-size:15.5px}
.abt-tools{display:flex;flex-wrap:wrap;gap:6px;margin-bottom:12px}
.abt-tools span{font-size:13.5px;font-weight:700;border:1.5px solid var(--line);border-radius:6px;padding:3px 9px}
.abt p.abt-lang{font-size:14.5px;color:var(--muted);margin:0}
.abt-refs li{font-size:14px;line-height:1.45;padding-left:28px!important;text-indent:-28px;margin:0 0 9px!important}
.abt-refs li b{font-weight:700}
.abt .abt-refs a{text-decoration:none;border-bottom:1.5px solid var(--acc)}
.abt .abt-refs a:hover{color:var(--acc)}
.abt-refs .n{display:inline-block;width:28px;text-indent:0;color:var(--muted);font-weight:700}

.abt mark.k{background:none;color:inherit;padding:0;transition:background .25s}
.abt-sheet.skim .abt-cols *{color:var(--dim)!important;transition:color .25s}
.abt-sheet.skim .abt-cols mark.k{color:var(--ink)!important;background:var(--acc-soft);box-shadow:0 0 0 2px var(--acc-soft);border-radius:2px}
.abt-sheet.skim .abt-cols .abt-h,.abt-sheet.skim .abt-cols .abt-h *{color:var(--on-grn)!important}
.abt-sheet.skim .abt-cols .abt-h span{color:var(--grn)!important}
.abt-sheet.skim .abt-cols .abt-fig *{color:var(--ink)!important}

@media(max-width:860px){.abt-cols{grid-template-columns:1fr 1fr}.abt-col:nth-child(2){border-right:0}.abt-col:nth-child(3){grid-column:span 2;border-top:1.5px solid var(--line)}}
@media(max-width:600px){.abt{padding:10px;font-size:16px}.abt-banner{grid-template-columns:1fr;padding:34px 22px 22px}.abt-ribbon{align-items:flex-start;flex-direction:row;flex-wrap:wrap}.abt-bar{padding:10px 22px}.abt-cols{grid-template-columns:1fr}.abt-col{border-right:0;border-top:1.5px solid var(--line);padding:22px}.abt-col:first-child{border-top:0}.abt-col:nth-child(3){grid-column:auto}}
@media(prefers-reduced-motion:reduce){.abt *{animation:none!important;transition:none!important}}
</style>
<div class="abt">
<div class="abt-sheet" id="abt-sheet">
  <div class="abt-banner">
    <div>
      <h1 class="abt-title">How much do people explain when they <mark>talk to a machine?</mark></h1>
      <p class="abt-authors">Hande Sodacı, PhD<sup>1</sup> · User experience &amp; behavioral researcher · Istanbul<br><sup>1</sup>Department of Psychology, Koç University</p>
    </div>
    <div class="abt-ribbon">
      <span class="open">Open to UX and behavioral research roles</span>
      <span class="hot">★ HRI '26 · Honorable Mention</span>
    </div>
  </div>
  <div class="abt-bar"><span>An about page, laid out as a research poster.</span><button type="button" class="abt-skim" id="abt-skim" aria-pressed="false">Skim it in 30 seconds</button></div>
  <div class="abt-cols">
    <div class="abt-col">
      <div class="abt-sec">
        <h2 class="abt-h"><span>1</span>Introduction</h2>
        <p>That is the question my PhD asked. I am a behavioral scientist with <mark class="k">a PhD in cognitive psychology from Koç University</mark> and <mark class="k">6+ years of experience investigating how people respond to and interact with technology</mark>, including social robots and tablet-based systems.</p>
        <p>I combine qualitative and quantitative methods across the full research cycle, from study design and data collection to reporting.</p>
      </div>
      <div class="abt-sec">
        <h2 class="abt-h"><span>2</span>Background</h2>
        <table class="abt-bg">
          <tr><td>2011–16</td><td><b>Boğaziçi University</b><span>BA in Psychology, with a certificate in Linguistics</span></td></tr>
          <tr><td>2016–18</td><td><b>Radboud University</b><span>Research Master in Language and Communication, Nijmegen</span></td></tr>
          <tr class="hl"><td>2017–18</td><td><b>Tilburg University</b><span>Research assistant on the EU Horizon 2020 <a href="/projects/robots-as-tutors/">L2TOR</a> project: a NAO robot teaching Dutch words to Turkish–Dutch children</span><em>Where my interest in human–robot interaction started</em></td></tr>
          <tr><td>2020–22</td><td><b>MEF University</b><span>Project coordinator for a TÜBİTAK-funded longitudinal study</span></td></tr>
          <tr><td>2020–26</td><td><b>Koç University</b><span>PhD in Psychology (Cognitive Track): in-lab studies of how people talk to human and robot listeners</span></td></tr>
          <tr><td>2023–25</td><td><b>European Open Science</b><span>Editorial assistant for 15 academic journals (remote)</span></td></tr>
        </table>
      </div>
    </div>
    <div class="abt-col">
      <div class="abt-sec">
        <h2 class="abt-h"><span>3</span>Methods</h2>
        <div class="abt-m"><h3>Testing</h3><p>I design and run <mark class="k">controlled in-lab user studies</mark>, from protocol design to data collection. My dissertation studies involved <mark class="k">200+ participants and 6,000+ responses</mark>.</p></div>
        <div class="abt-m"><h3>Analyzing</h3><p>I model user behavior trial by trial with <mark class="k">mixed-effects and ordinal models in R</mark>, using reproducible workflows, and I report what the data show even when it is not what I expected.</p></div>
        <div class="abt-m"><h3>Building</h3><p>I <mark class="k">program the robot interactions</mark> for my studies and pilot each task over several rounds until it feels natural to users. When existing measures could not capture what I was looking for, I <mark class="k">developed a new one</mark>. I also hold an Associate Degree in Web Design and Coding and set up this site myself.</p></div>
        <div class="abt-m"><h3>Communicating</h3><p>I prepare visually structured reports, presentations, and posters <mark class="k">for technical and non-technical audiences</mark>, including my ACM/IEEE HRI 2026 poster, which received an Honorable Mention.</p></div>
      </div>
      <div class="abt-sec">
        <h2 class="abt-h"><span>4</span>Materials</h2>
        <div class="abt-tools"><span>R</span><span>SPSS</span><span>JASP</span><span>Qualtrics</span><span>OpenSesame</span><span>ELAN</span><span>Choregraphe (NAO)</span><span>HTML/CSS</span><span>Microsoft Office</span></div>
        <p class="abt-lang"><b>Languages:</b> Turkish (native), English (fluent)</p>
      </div>
    </div>
    <div class="abt-col">
      <div class="abt-sec">
        <h2 class="abt-h"><span>5</span>Results</h2>
        <div class="abt-res">
          <p>People gave a robot more detail than a human listener who behaved the same way (Fig. 1). They did not say less once the robot began guessing correctly, and <mark class="k">gave more detail only when it explicitly failed to understand them</mark>.</p>
          <div class="abt-fig" data-fig>
            <div class="row"><span>Human</span><span class="track"><i style="--w:66%"></i></span><span>1.98</span></div>
            <div class="row"><span>Robot</span><span class="track"><i class="a" style="--w:74.3%"></i></span><span>2.23</span></div>
            <p class="abt-cap"><b>Fig. 1.</b> Average detail per description, by listener.</p>
          </div>
          <a class="abt-more" href="/projects/talking-to-robots/">Talking to Robots →</a>
        </div>
        <div class="abt-res">
          <p>Most children preferred the robot that also spoke Turkish (Fig. 2), yet they learned more from the one that spoke only Dutch. That taught me to <mark class="k">separate what users like from what works for them</mark>.</p>
          <div class="abt-fig" data-fig>
            <div class="row"><span>Bilingual</span><span class="track"><i class="a" style="--w:72%"></i></span><span>72%</span></div>
            <div class="row"><span>Dutch-only</span><span class="track"><i style="--w:28%"></i></span><span>28%</span></div>
            <p class="abt-cap"><b>Fig. 2.</b> Which robot children wanted to play with again.</p>
          </div>
          <a class="abt-more" href="/projects/robots-as-tutors/">Robots as Tutors →</a>
        </div>
      </div>
      <div class="abt-sec abt-disc">
        <h2 class="abt-h"><span>6</span>Discussion</h2>
        <p>I want to bring my research experience to <mark class="k">usability testing and other user studies of interactive products</mark>, turning evidence from real users into actionable insights for engineers and designers.</p>
      </div>
      <div class="abt-sec">
        <h2 class="abt-h"><span>7</span>References</h2>
        <ol class="abt-refs">
          <li><span class="n">[1]</span>Sodacı, H. <a href="/projects/talking-to-robots/"><b>Talking to Robots</b></a>. Project page.</li>
          <li><span class="n">[2]</span>Sodacı, H. <a href="/projects/robots-as-tutors/"><b>Robots as Tutors</b></a>. Project page.</li>
          <li><span class="n">[3]</span>Sodacı, H. (2026). <a href="/assets/HS_resume_202611.pdf"><b>Resume</b></a> [PDF].</li>
          <li><span class="n">[4]</span>Sodacı, H. <a href="/contact/"><b>Get in touch</b></a>. Contact form.</li>
        </ol>
      </div>
    </div>
  </div>
</div>
</div>
<script>
(function () {
  var root = document.querySelector(".abt");
  if (!root) { return; }
  var sheet = document.getElementById("abt-sheet");
  var skim = document.getElementById("abt-skim");
  skim.addEventListener("click", function () {
    var on = !sheet.classList.contains("skim");
    sheet.classList.toggle("skim", on);
    skim.setAttribute("aria-pressed", on ? "true" : "false");
    skim.textContent = on ? "Show everything" : "Skim it in 30 seconds";
  });
  var figs = [].slice.call(root.querySelectorAll("[data-fig]"));
  if ("IntersectionObserver" in window && !matchMedia("(prefers-reduced-motion: reduce)").matches) {
    var io = new IntersectionObserver(function (es) {
      es.forEach(function (e) { if (e.isIntersecting) { e.target.classList.add("on"); io.unobserve(e.target); } });
    }, { threshold: 0.4 });
    figs.forEach(function (f) { io.observe(f); });
  } else {
    figs.forEach(function (f) { f.classList.add("on"); });
  }
})();
</script>
