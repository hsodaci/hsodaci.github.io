---
title: About
permalink: /about/
layout: page
excerpt: Behavioral researcher with a recent PhD in Psychology (Cognitive Track) from Koç University, moving that experimental mindset into product and research work.
comments: false
---
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:wght@400;600&family=IBM+Plex+Sans:wght@400;500;600;700&display=swap" rel="stylesheet">
<style>
/* About page as a rendered R notebook: text and outputs first, code folded away. Every rule is scoped to .abt and every class is prefixed abt-. Fonts: IBM Plex Sans for text, IBM Plex Mono for code. */
.header:has(+ .page-content .abt){display:none}
.abt{--bg:#ffffff;--page:#f4f5f7;--ink:#1f2328;--muted:#5f6670;--line:rgba(31,35,40,.12);--chunk:#f6f8fa;--kw:#8250df;--fn:#0550ae;--str:#116329;--com:#6e7781;--pn:#ebebeb;--grid:#ffffff;--acc:#00B0F6;
  font-family:"IBM Plex Sans",system-ui,-apple-system,"Segoe UI",Roboto,sans-serif;font-size:17.5px;line-height:1.65;color:var(--ink);text-align:left;max-width:820px;margin:0 auto;padding:0}
body[data-theme="dark"] .abt{--bg:#1b1d23;--page:#121418;--ink:#e6e6e3;--muted:#a3a8b1;--line:rgba(230,230,227,.12);--chunk:#252932;--kw:#c4a5ff;--fn:#79b8ff;--str:#9ecf8f;--com:#8b949e;--pn:#2a2e37;--grid:#3a3f4a}
.abt *,.abt *::before,.abt *::after{box-sizing:border-box}
.abt p{margin:0 0 14px;padding:0;color:inherit;opacity:1}
.abt h1,.abt h2{font-family:inherit;color:inherit;margin:0;padding:0;border:0;letter-spacing:normal;text-transform:none}
.abt h2::before,.abt h2::after{content:none}
.abt a{color:inherit}
.abt a::after{content:none!important}
.abt b,.abt strong{color:inherit!important}
.abt pre,.abt code{font-family:"IBM Plex Mono",ui-monospace,Menlo,Consolas,monospace;background:none!important;border:0!important;padding:0!important;margin:0;color:inherit;box-shadow:none!important}

.abt-doc{background:var(--bg);border:1px solid var(--line);border-radius:12px;padding:44px 52px 40px;box-shadow:0 18px 40px -26px rgba(0,0,0,.35)}
.abt-file{display:flex;align-items:center;gap:8px;font-family:"IBM Plex Mono",monospace;font-size:13px;color:var(--muted);margin-bottom:26px}
.abt-file span{border:1px solid var(--line);border-radius:5px;padding:2px 8px}
.abt h1.abt-title{font-weight:700;font-size:clamp(34px,5vw,46px);line-height:1.1;letter-spacing:-.02em;margin-bottom:6px}
.abt p.abt-subt{font-size:19px;color:var(--muted);margin-bottom:6px}
.abt p.abt-meta{font-size:14px;color:var(--muted);margin-bottom:30px}
.abt h2.abt-h2{font-weight:700;font-size:24px;letter-spacing:-.01em;margin:38px 0 12px;padding-bottom:6px;border-bottom:1px solid var(--line)}

.abt details.abt-code{margin:10px 0 8px}
.abt details.abt-code summary{display:inline-flex;align-items:center;gap:6px;font-family:"IBM Plex Mono",monospace;font-size:13px;color:var(--muted);cursor:pointer;list-style:none;padding:2px 0;user-select:none}
.abt details.abt-code summary::-webkit-details-marker{display:none}
.abt details.abt-code summary::before{content:"▸";display:inline-block;transition:transform .15s}
.abt details.abt-code[open] summary::before{transform:rotate(90deg)}
.abt details.abt-code summary:hover{color:var(--ink)}
.abt pre.abt-chunk{display:block;background:var(--chunk)!important;border-left:3px solid var(--line)!important;border-radius:4px;padding:12px 16px!important;margin-top:8px!important;font-size:14px;line-height:1.6;white-space:pre;overflow-x:auto}
.abt .k{color:var(--kw)}.abt .f{color:var(--fn)}.abt .s{color:var(--str)}.abt .c{color:var(--com)}

.abt-q{font-weight:600;font-size:clamp(22px,3.2vw,28px);line-height:1.3;letter-spacing:-.01em;border-left:4px solid var(--acc);padding:4px 0 4px 18px;margin:8px 0 6px}
.abt-out{margin:6px 0 4px}
.abt-plot{display:block;width:100%;height:auto;margin:4px 0}
.abt-plot .pn{fill:var(--pn)}
.abt-plot .gl{stroke:var(--grid);stroke-width:1.4}
.abt-plot .gm{stroke:var(--grid);stroke-width:.7;opacity:.7}
.abt-plot .ax{fill:var(--muted);font-family:"IBM Plex Sans",sans-serif;font-size:13px}
.abt-plot .axt{fill:var(--ink);font-family:"IBM Plex Sans",sans-serif;font-size:14px}
.abt-plot .lb{fill:var(--ink);font-family:"IBM Plex Sans",sans-serif;font-weight:600;font-size:14.5px}
.abt-plot .bar{stroke-width:11;stroke-linecap:round;stroke-dasharray:var(--len,600);stroke-dashoffset:var(--len,600);transition:stroke-dashoffset 1s cubic-bezier(.2,.8,.2,1)}
.abt-plot .bar.nx{stroke-width:5;stroke-dasharray:3 9;stroke-dashoffset:0}
.abt-plot .arw{fill:none;stroke-width:3.5;stroke-linecap:round;stroke-linejoin:round}
.abt-plot.on .bar{stroke-dashoffset:0}
.abt p.abt-cap{font-size:14px;color:var(--muted)}

.abt-call{display:flex;gap:14px;align-items:flex-start;border:1px solid var(--line);border-left:4px solid #E76BF3;border-radius:6px;padding:14px 16px;margin:8px 0 4px;background:color-mix(in srgb,#E76BF3 7%,transparent)}
.abt-call b{display:block;font-weight:700;font-size:15px;color:#a63fb0!important;margin-bottom:2px}
body[data-theme="dark"] .abt-call b{color:#f0a3f5!important}
.abt-call p{margin:0;font-size:17px}
.abt-links{display:flex;flex-wrap:wrap;gap:10px;margin-top:30px}
.abt a.abt-btn{font-weight:600;font-size:15.5px;text-decoration:none;color:var(--ink)!important;border:1px solid var(--line);border-radius:8px;padding:9px 16px;transition:border-color .15s,background .15s}
.abt a.abt-btn:hover{border-color:var(--fn);background:var(--chunk)}
.abt a.abt-btn code{font-size:14px;color:var(--fn)}
@media(max-width:640px){.abt-plot .lb{font-size:27px}.abt-plot .ax,.abt-plot .axt{font-size:22px}.abt{font-size:16.5px}.abt-doc{padding:28px 20px 26px;border-radius:10px}.abt-chunk{font-size:12.5px}}
@media(prefers-reduced-motion:reduce){.abt-plot .bar{transition:none;stroke-dashoffset:0}}
</style>
<div class="abt">
<div class="abt-doc">
  <div class="abt-file"><span>about.qmd</span>rendered notebook</div>
  <h1 class="abt-title">About</h1>
  <p class="abt-subt">A short notebook, not a CV.</p>
  <p class="abt-meta">Read the text and the outputs. The code is folded away, for the curious.</p>

  <h2 class="abt-h2">The question</h2>
  <p>My PhD asked one question:</p>
  <div class="abt-out"><p class="abt-q">How much do people explain when they talk to a machine?</p></div>
  <details class="abt-code"><summary>Code</summary><pre class="abt-chunk">hande <span class="k">&lt;-</span> <span class="f">researcher</span>(
&nbsp;&nbsp;field&nbsp;&nbsp;&nbsp;&nbsp;= <span class="s">"UX and behavioral research"</span>,
&nbsp;&nbsp;question = <span class="s">"How much do people explain when they talk to a machine?"</span>
)
hande<span class="k">$</span>question</pre></details>
  <p>The short answer from my studies: people gave a robot more detail than a person, and they did not explain less when the robot kept getting it right. Only a clear "I didn't get that" made them explain more.</p>

  <h2 class="abt-h2">The path so far</h2>
  <p>Five stops, from psychology in Istanbul to robots in the Netherlands and back.</p>
  <div class="abt-out"><svg class="abt-plot" viewBox="0 0 660 300" role="img" aria-label="Timeline: Psychology BA at Boğaziçi 2011 to 2016, research master at Radboud 2016 to 2018, first robot at Tilburg 2017 to 2018, PhD at Koç University 2020 to 2026, next: UX research from 2026."><rect class="pn" x="16" y="14" width="628" height="246"/><line class="gm" x1="89.9" x2="89.9" y1="14" y2="260"/><line class="gm" x1="163.8" x2="163.8" y1="14" y2="260"/><line class="gm" x1="237.6" x2="237.6" y1="14" y2="260"/><line class="gm" x1="311.5" x2="311.5" y1="14" y2="260"/><line class="gm" x1="385.4" x2="385.4" y1="14" y2="260"/><line class="gm" x1="459.3" x2="459.3" y1="14" y2="260"/><line class="gm" x1="533.2" x2="533.2" y1="14" y2="260"/><line class="gm" x1="607.1" x2="607.1" y1="14" y2="260"/><line class="gl" x1="52.9" x2="52.9" y1="14" y2="260"/><text class="ax" x="52.9" y="280" text-anchor="middle">2012</text><line class="gl" x1="126.8" x2="126.8" y1="14" y2="260"/><text class="ax" x="126.8" y="280" text-anchor="middle">2014</text><line class="gl" x1="200.7" x2="200.7" y1="14" y2="260"/><text class="ax" x="200.7" y="280" text-anchor="middle">2016</text><line class="gl" x1="274.6" x2="274.6" y1="14" y2="260"/><text class="ax" x="274.6" y="280" text-anchor="middle">2018</text><line class="gl" x1="348.5" x2="348.5" y1="14" y2="260"/><text class="ax" x="348.5" y="280" text-anchor="middle">2020</text><line class="gl" x1="422.4" x2="422.4" y1="14" y2="260"/><text class="ax" x="422.4" y="280" text-anchor="middle">2022</text><line class="gl" x1="496.2" x2="496.2" y1="14" y2="260"/><text class="ax" x="496.2" y="280" text-anchor="middle">2024</text><line class="gl" x1="570.1" x2="570.1" y1="14" y2="260"/><text class="ax" x="570.1" y="280" text-anchor="middle">2026</text><line class="bar" x1="16.0" x2="200.7" y1="44.5" y2="44.5" stroke="#F8766D"/><text class="lb" x="16.0" y="30.5">Psychology BA · Boğaziçi</text><line class="bar" x1="200.7" x2="274.6" y1="93.7" y2="93.7" stroke="#A3A500"/><text class="lb" x="200.7" y="79.7">Research master · Radboud</text><line class="bar" x1="237.6" x2="274.6" y1="142.9" y2="142.9" stroke="#00BF7D"/><text class="lb" x="237.6" y="128.9">First robot · Tilburg</text><line class="bar" x1="348.5" x2="570.1" y1="192.1" y2="192.1" stroke="#00B0F6"/><text class="lb" x="348.5" y="178.1">PhD · Koç University</text><line class="bar nx" x1="570.1" x2="636.0" y1="241.3" y2="241.3" stroke="#E76BF3"/><path class="arw" d="M632.0 234.3L642.0 241.3L632.0 248.3" stroke="#E76BF3"/><text class="lb" x="642.0" y="227.3" text-anchor="end">Next: UX research</text><text class="axt" x="330" y="296" text-anchor="middle">year</text></svg></div>
  <details class="abt-code"><summary>Code</summary><pre class="abt-chunk"><span class="f">ggplot</span>(path, <span class="f">aes</span>(x <span class="k">=</span> start, xend <span class="k">=</span> end, y <span class="k">=</span> stop)) <span class="k">+</span>
&nbsp;&nbsp;<span class="f">geom_segment</span>(linewidth <span class="k">=</span> 4, lineend <span class="k">=</span> <span class="s">"round"</span>) <span class="k">+</span>
&nbsp;&nbsp;<span class="f">labs</span>(x <span class="k">=</span> <span class="s">"year"</span>, y <span class="k">=</span> <span class="k">NULL</span>) <span class="c"># the last stop has no end date yet</span></pre></details>

  <h2 class="abt-h2">What's next</h2>
  <div class="abt-out"><div class="abt-call"><div><b>next_step()</b><p>UX research: how real people experience interactive products.</p></div></div></div>
  <details class="abt-code"><summary>Code</summary><pre class="abt-chunk"><span class="f">next_step</span>(hande)</pre></details>

  <div class="abt-links">
    <a class="abt-btn" href="/projects/talking-to-robots/">See my projects</a>
    <a class="abt-btn" href="/assets/HS_resume_202611.pdf">Resume <code>.pdf</code></a>
    <a class="abt-btn" href="/contact/">Say hello</a>
  </div>
</div>
</div>
<script>
(function () {
  var plot = document.querySelector(".abt .abt-plot");
  if (!plot) { return; }
  [].forEach.call(plot.querySelectorAll(".bar:not(.nx)"), function (b) {
    b.style.setProperty("--len", Math.ceil(b.getTotalLength() + 20));
  });
  if ("IntersectionObserver" in window && !matchMedia("(prefers-reduced-motion: reduce)").matches) {
    var io = new IntersectionObserver(function (es) {
      if (es[0].isIntersecting) { io.disconnect(); plot.classList.add("on"); }
    }, { threshold: 0.4 });
    io.observe(plot);
  } else { plot.classList.add("on"); }
})();
</script>
