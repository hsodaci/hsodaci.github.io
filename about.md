---
title: About
permalink: /about/
layout: page
excerpt: Behavioral researcher with a recent PhD in Psychology (Cognitive Track) from Koç University, moving that experimental mindset into product and research work.
comments: false
---
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;600;700&display=swap" rel="stylesheet">
<style>
/* About page as an R console. Every rule is scoped to .abt and every class is prefixed abt-. One monospace font (JetBrains Mono). */
.header:has(+ .page-content .abt){display:none}
.abt{--page:#f3f4f6;--bg:#ffffff;--bar:#e9ebef;--ink:#1f2328;--dim:#6e7781;--pr:#0550ae;--str:#116329;--num:#953800;--err:#cf222e;--hl:#ddf4ff;--line:rgba(31,35,40,.12);
  font-family:"JetBrains Mono",ui-monospace,SFMono-Regular,Menlo,Consolas,monospace;font-size:15px;line-height:1.55;color:var(--ink);text-align:left;max-width:920px;margin:0 auto;padding:22px;background:var(--page);border-radius:14px}
body[data-theme="dark"] .abt{--page:#111315;--bg:#1d1f21;--bar:#282a2e;--ink:#c5c8c6;--dim:#8a8f94;--pr:#81a2be;--str:#b5bd68;--num:#de935f;--err:#cc6666;--hl:#2d3a46;--line:rgba(197,200,198,.12)}
.abt *,.abt *::before,.abt *::after{box-sizing:border-box}
.abt p{margin:0;padding:0;color:inherit}
.abt h1{position:absolute;width:1px;height:1px;overflow:hidden;clip:rect(0 0 0 0);white-space:nowrap;margin:0;padding:0;border:0}
.abt a{color:inherit}
.abt a::after{content:none!important}
.abt b,.abt strong{color:inherit!important}
.abt pre,.abt code{font-family:inherit;font-size:inherit;background:none!important;border:0!important;padding:0!important;margin:0;color:inherit;white-space:pre;box-shadow:none!important}
.abt button,.abt input{font-family:inherit}

.abt-win{background:var(--bg);border-radius:10px;border:1px solid var(--line);box-shadow:0 20px 40px -24px rgba(0,0,0,.45);overflow:hidden}
.abt-tabs{display:flex;align-items:center;gap:2px;background:var(--bar);border-bottom:1px solid var(--line);padding:6px 10px 0}
.abt-tabs span{font-size:12.5px;padding:6px 12px;border-radius:6px 6px 0 0;color:var(--dim)}
.abt-tabs span.on{background:var(--bg);color:var(--ink);font-weight:600}
.abt-tabs i{margin-left:auto;font-style:normal;font-size:12px;color:var(--dim);padding-bottom:6px}
.abt-tabs button{font-size:12px;border:1px solid var(--line);background:var(--bg);color:var(--dim);border-radius:5px;padding:2px 8px;margin:0 0 6px 10px;cursor:pointer}
.abt-con{padding:16px 18px 18px;min-height:420px;overflow-x:auto}
.abt-con pre{line-height:1.55}
.abt-cmd{display:block;color:var(--ink)}
.abt-cmd::before{content:"> ";color:var(--pr);font-weight:700}
.abt-out{display:block;margin:2px 0 14px;color:var(--ink)}
.abt .abt-c{color:var(--dim)}
.abt .abt-s{color:var(--str)}
.abt .abt-n{color:var(--num)}
.abt .abt-e{color:var(--err)}
.abt-h{font-weight:700}
.abt-out button.abt-fn{border:0;background:none;padding:0;color:var(--pr);text-decoration:underline;text-underline-offset:3px;cursor:pointer;font-size:inherit}
.abt-caret{display:inline-block;width:.6em;height:1.1em;vertical-align:-.2em;background:var(--ink);animation:abt-blink 1s steps(1) infinite}
@keyframes abt-blink{50%{opacity:0}}
.abt-form{display:flex;align-items:center;gap:0}
.abt-form label{color:var(--pr);font-weight:700;white-space:pre}
.abt-form input{flex:1;min-width:0;border:0;outline:0;background:transparent;color:var(--ink);font-size:inherit;padding:0;caret-color:var(--ink)}
.abt-chips{display:flex;flex-wrap:wrap;gap:8px;margin-top:14px;padding-top:12px;border-top:1px dashed var(--line)}
.abt-chips span{font-size:12.5px;color:var(--dim);align-self:center;margin-right:4px}
.abt-chips button{font-size:13px;border:1px solid var(--line);background:var(--bar);color:var(--ink);border-radius:6px;padding:5px 10px;cursor:pointer;transition:background .15s,border-color .15s}
.abt-chips button:hover{background:var(--hl);border-color:var(--pr)}
.abt-hide{display:none}
@media(max-width:600px){.abt .abt-con pre{white-space:pre-wrap;overflow-wrap:anywhere}.abt{padding:8px;font-size:12px}.abt-con{padding:12px;min-height:360px}.abt-tabs span:not(.on){display:none}}
@media(prefers-reduced-motion:reduce){.abt-caret{animation:none}}
</style>
<div class="abt">
<h1>About</h1>
<div class="abt-win">
  <div class="abt-tabs"><span class="on">Console</span><span>Terminal</span><span>Background Jobs</span><i>~/hsodaci/about/</i><button type="button" id="abt-skip">skip</button></div>
  <div class="abt-con" id="abt-con" aria-live="polite">
    <div id="abt-log"></div>
    <form class="abt-form abt-hide" id="abt-form" autocomplete="off"><label for="abt-in">&gt; </label><input id="abt-in" type="text" spellcheck="false" aria-label="Type an R command"></form>
    <div class="abt-chips abt-hide" id="abt-chips"><span># try</span><button type="button" data-c="?hande">?hande</button><button type="button" data-c="path()">path()</button><button type="button" data-c="next_step()">next_step()</button><button type="button" data-c="ls()">ls()</button><button type="button" data-c="projects()">projects()</button><button type="button" data-c="resume()">resume()</button><button type="button" data-c="contact()">contact()</button></div>
  </div>
</div>
</div>
<script>
(function () {
  var root = document.querySelector(".abt");
  if (!root) { return; }
  var log = document.getElementById("abt-log");
  var form = document.getElementById("abt-form");
  var input = document.getElementById("abt-in");
  var chips = document.getElementById("abt-chips");
  var con = document.getElementById("abt-con");
  var reduce = matchMedia("(prefers-reduced-motion: reduce)").matches;

  function fn(name) { return '<button type="button" class="abt-fn" data-c="' + name + '">' + name + '</button>'; }
  function sp(n) { return new Array(n + 1).join(" "); }
  function pad(t, n) { return t + sp(Math.max(1, n - t.length)); }
  var C = function (t) { return '<span class="abt-c">' + t + '</span>'; };
  var S = function (t) { return '<span class="abt-s">' + t + '</span>'; };
  var H = function (t) { return '<span class="abt-h">' + t + '</span>'; };
  var I5 = sp(5);
  var rows = [["Boğaziçi", "2011–16", "Psychology, plus a linguistics certificate"],
              ["Radboud", "2016–18", "Research master in language and communication"],
              ["Tilburg", "2017–18", "First robot (L2TOR): Dutch words for kids"],
              ["Koç", "2020–26", "PhD: how much people explain to machines"],
              ["???", "NA", "UX research"]];
  var tib = C("# A tibble: 5 × 3") + "\n" + sp(2) + pad("stop", 9) + pad("years", 9) + "what\n" + sp(2) + C(pad("&lt;chr&gt;", 18).replace(/ +$/, "")).replace("&lt;chr&gt;", "&lt;chr&gt;") ;
  tib = C("# A tibble: 5 × 3") + "\n" + sp(2) + pad("stop", 9) + pad("years", 9) + "what\n" + sp(2) + C("&lt;chr&gt;" + sp(4) + "&lt;chr&gt;" + sp(4) + "&lt;chr&gt;");
  rows.forEach(function (r, i) {
    var yr = r[1] === "NA" ? '<span class="abt-e">NA</span>' + sp(7) : pad(r[1], 9);
    tib += "\n" + C(String(i + 1)) + " " + pad(r[0], 9) + yr + r[2];
  });
  var OUT = {
    "?hande": C("hande" + sp(21) + "package:koc" + sp(20) + "R Documentation") + "\n\n" + H("Hande Sodacı, PhD") + "\n\n" + H("Description:") + "\n\n" + I5 + "A UX and behavioral researcher who studies how much people\n" + I5 + "explain when they talk to a machine.\n\n" + H("Usage:") + "\n\n" + I5 + "hande(question, users = " + S('"real"') + ', robot = <span class="abt-n">TRUE</span>)\n\n' + H("Arguments:") + "\n\n" + sp(1) + pad("question", 10) + "something about how people behave with technology.\n" + sp(1) + pad("users", 10) + "preferably real ones.\n" + sp(1) + pad("robot", 10) + "optional, but encouraged.\n\n" + H("Value:") + "\n\n" + I5 + "Controlled studies, tidy R code, and findings that engineers\n" + I5 + "and designers can act on.\n\n" + H("See Also:") + "\n\n" + I5 + fn("path()") + ", " + fn("next_step()") + ", " + fn("projects()"),
    "path()": tib,
    "next_step()": C("[1]") + " " + S('"UX research: how real people experience interactive products"'),
    "ls()": C("[1]") + " " + [S('"contact"'), S('"next_step"'), S('"path"'), S('"projects"'), S('"resume"')].join(" "),
    "projects()": C('Opening "Talking to Robots" and "Robots as Tutors"...'),
    "resume()": C("Opening HS_resume_202611.pdf..."),
    "contact()": C("Opening the contact form...")
  };
  var GO = { "projects()": "/projects/talking-to-robots/", "resume()": "/assets/HS_resume_202611.pdf", "contact()": "/contact/" };
  var ALIAS = { "help(hande)": "?hande", "?hande()": "?hande", "path": "path()", "next_step": "next_step()", "ls": "ls()" };

  function line(cls, html) {
    var p = document.createElement("pre");
    p.className = cls;
    p.innerHTML = html;
    log.appendChild(p);
    con.scrollTop = con.scrollHeight;
    return p;
  }
  function esc(s) { return s.replace(/&/g, "&amp;").replace(/</g, "&lt;").replace(/>/g, "&gt;"); }
  function run(cmd) {
    var c = cmd.trim();
    if (!c) { line("abt-cmd", ""); return; }
    var k = ALIAS[c] || c;
    line("abt-cmd", esc(c));
    if (k === "clear()" || k === "cat(\"\\014\")") { log.innerHTML = ""; return; }
    if (OUT[k]) {
      line("abt-out", OUT[k]);
      if (GO[k]) { setTimeout(function () { location.href = GO[k]; }, 700); }
      return;
    }
    var m = c.match(/^([A-Za-z_.][A-Za-z0-9_.]*)\s*\(/);
    if (m) { line("abt-out abt-e", "Error in " + esc(m[1]) + "() : could not find function \"" + esc(m[1]) + "\""); }
    else { line("abt-out abt-e", "Error: object '" + esc(c.split(/\s/)[0]) + "' not found"); }
  }

  var script = ["?hande", "path()", "next_step()"];
  var timers = [];
  var done = false;
  function later(f, ms) { timers.push(setTimeout(f, ms)); }
  function finish() {
    if (done) { return; }
    done = true;
    timers.forEach(clearTimeout);
    log.innerHTML = "";
    line("abt-out abt-c", "# about.R: a sketch, not a CV. For the full version, run resume().");
    script.forEach(function (c) { line("abt-cmd", esc(c)); line("abt-out", OUT[c]); });
    form.classList.remove("abt-hide");
    chips.classList.remove("abt-hide");
    document.getElementById("abt-skip").style.display = "none";
  }
  function typeOut(i) {
    if (i >= script.length) { later(finish, 400); return; }
    var c = script[i];
    var p = line("abt-cmd", "");
    var caret = '<span class="abt-caret"></span>';
    var n = 0;
    (function tick() {
      n++;
      p.innerHTML = esc(c.slice(0, n)) + (n < c.length ? caret : "");
      if (n < c.length) { later(tick, 70); }
      else { later(function () { line("abt-out", OUT[c]); later(function () { typeOut(i + 1); }, 900); }, 250); }
    })();
  }
  function start() {
    if (reduce) { finish(); return; }
    line("abt-out abt-c", "# about.R: a sketch, not a CV. For the full version, run resume().");
    later(function () { typeOut(0); }, 500);
  }
  document.getElementById("abt-skip").addEventListener("click", finish);
  form.addEventListener("submit", function (e) { e.preventDefault(); run(input.value); input.value = ""; });
  root.addEventListener("click", function (e) {
    var b = e.target.closest("[data-c]");
    if (!b || !done) { return; }
    run(b.getAttribute("data-c"));
  });
  if ("IntersectionObserver" in window) {
    var io = new IntersectionObserver(function (es) {
      if (es[0].isIntersecting) { io.disconnect(); start(); }
    }, { threshold: 0.3 });
    io.observe(con);
  } else { start(); }
})();
</script>
