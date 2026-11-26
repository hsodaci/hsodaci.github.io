---
title: About
permalink: /about/
layout: page
excerpt: Behavioral researcher with a recent PhD in Psychology (Cognitive Track) from Koç University, moving that experimental mindset into product and research work.
comments: false
---
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@500;600;700&display=swap" rel="stylesheet">
<style>
/* About page as a cross-stitch sampler. Every rule is scoped to .abt and every class is prefixed abt-. One font (Quicksand). The stitched motifs are drawn by the script at the bottom. */
.header:has(+ .page-content .abt){display:none}
.abt{--wall:#f7f1e6;--ink:#3a3330;--muted:#7b716a;--linen:#f1e7d3;--grid:rgba(122,90,58,.09);--red:#c8463d;--grn:#4f7a4a;--blu:#3c6aa8;--mus:#d9a441;--wood:#c9935c;--wood2:#a8733f;
  background:var(--wall);color:var(--ink);font-family:"Quicksand",system-ui,-apple-system,"Segoe UI",Roboto,sans-serif;font-weight:500;font-size:18px;line-height:1.6;text-align:left;max-width:900px;margin:0 auto;padding:24px 30px 56px;border-radius:18px}
body[data-theme="dark"] .abt{--wall:#1e1a17;--ink:#efe6d8;--muted:#b3a698}
.abt *,.abt *::before,.abt *::after{box-sizing:border-box}
.abt p{margin:0;padding:0;color:inherit;opacity:1}
.abt h1,.abt h2{font-family:inherit;color:inherit;margin:0;padding:0;border:0;letter-spacing:normal;text-transform:none}
.abt h2::before,.abt h2::after{content:none}
.abt a{color:inherit}
.abt a::after{content:none!important}
.abt b,.abt strong{color:inherit!important}
.abt-cloth{background-color:var(--linen);background-image:repeating-linear-gradient(0deg,var(--grid) 0 1px,transparent 1px 9px),repeating-linear-gradient(90deg,var(--grid) 0 1px,transparent 1px 9px)}

.abt-top{display:grid;grid-template-columns:auto 1fr;gap:44px;align-items:center;padding:30px 0 10px}
.abt-hoop{position:relative;width:330px;height:330px;border-radius:50%;padding:14px;background:linear-gradient(145deg,var(--wood),var(--wood2));box-shadow:0 14px 30px -14px rgba(60,35,10,.5),inset 0 0 0 3px rgba(255,255,255,.18)}
.abt-hoop::before{content:"";position:absolute;left:50%;top:-16px;width:26px;height:26px;margin-left:-13px;border-radius:6px;background:linear-gradient(#b8bcc4,#7d828c);box-shadow:0 2px 3px rgba(0,0,0,.3)}
.abt-hoopin{width:100%;height:100%;border-radius:50%;display:grid;place-items:center;overflow:hidden;box-shadow:inset 0 0 0 5px var(--wood2),inset 0 6px 14px rgba(60,35,10,.25)}
.abt-hoopin svg{width:82%;height:auto;display:block}
.abt h1.abt-h1{font-weight:700;font-size:clamp(38px,6vw,58px);line-height:1.05;letter-spacing:-.02em;margin-bottom:16px}
.abt-h1 span{color:var(--red)}
body[data-theme="dark"] .abt-h1 span{color:#ef7a6f}
.abt p.abt-intro{font-size:20px;line-height:1.55;max-width:34ch;margin-bottom:12px}
.abt p.abt-note{font-size:16px;color:var(--muted);max-width:36ch}

.abt-sampler{position:relative;margin:56px 0 0;border-radius:6px;padding:34px 30px 30px;box-shadow:0 18px 34px -20px rgba(60,35,10,.45)}
.abt-sampler::before{content:"";position:absolute;inset:12px;border:2.5px dashed var(--red);border-radius:4px;pointer-events:none;opacity:.75}
.abt h2.abt-h2{position:relative;text-align:center;font-weight:700;font-size:15px;letter-spacing:.14em;text-transform:uppercase;color:#7a5a3a;margin-bottom:24px}
.abt-motifs{position:relative;display:grid;grid-template-columns:repeat(5,1fr);gap:18px}
.abt-m{position:relative;z-index:1;text-align:center;color:#3a3330}
.abt-m svg{display:block;height:118px;width:auto;max-width:100%;margin:0 auto 14px;overflow:visible}
.abt-m b{display:block;font-weight:700;font-size:13px;letter-spacing:.1em;text-transform:uppercase;color:#7a5a3a;margin-bottom:4px}
.abt-m p{font-size:15.5px;line-height:1.45;color:#3a3330}
.abt-m.next p{color:#7a5a3a}
.abt-needle{transform-origin:20% 80%;animation:abt-bob 2.4s ease-in-out infinite}
@keyframes abt-bob{0%,100%{transform:rotate(0)}50%{transform:rotate(-6deg) translateY(-2px)}}

.abt-patches{display:flex;flex-wrap:wrap;justify-content:center;gap:14px;margin-top:40px}
.abt a.abt-patch{position:relative;display:inline-block;text-decoration:none;font-weight:700;font-size:17px;color:#3a3330!important;padding:12px 22px;border-radius:12px;transform:rotate(var(--r,0deg));transition:transform .25s cubic-bezier(.34,1.56,.64,1);box-shadow:0 6px 12px -8px rgba(60,35,10,.5)}
.abt a.abt-patch::before{content:"";position:absolute;inset:5px;border:2px dashed var(--c,var(--red));border-radius:8px}
.abt a.abt-patch:hover{transform:rotate(0) translateY(-3px)}
.abt a.abt-patch:nth-child(1){--r:-2deg;--c:var(--red)}
.abt a.abt-patch:nth-child(2){--r:1.5deg;--c:var(--blu)}
.abt a.abt-patch:nth-child(3){--r:-1deg;--c:var(--grn)}

@media(max-width:760px){.abt-top{grid-template-columns:1fr;gap:28px;justify-items:center;text-align:center}.abt p.abt-intro,.abt p.abt-note{margin-left:auto;margin-right:auto}.abt-motifs{grid-template-columns:repeat(2,1fr);gap:26px 18px}.abt-m.next{grid-column:span 2}}
@media(max-width:420px){.abt{padding:14px 14px 40px}.abt-hoop{width:270px;height:270px}.abt-sampler{padding:30px 18px 24px}}
@media(prefers-reduced-motion:reduce){.abt-needle{animation:none}}
</style>
<div class="abt">
<div class="abt-top">
  <div class="abt-hoop" aria-hidden="true"><div class="abt-hoopin abt-cloth" id="abt-name"></div></div>
  <div>
    <h1 class="abt-h1">Hi, I'm <span>Hande.</span></h1>
    <p class="abt-intro">I'm a UX and behavioral researcher in Istanbul. My PhD asked how much people explain when they talk to a machine.</p>
  </div>
</div>
<div class="abt-sampler abt-cloth">
  <h2 class="abt-h2">My path so far</h2>
  <div class="abt-motifs">
    <div class="abt-m" data-motif="tulip"><b>Istanbul</b><p>Psychology at Boğaziçi, with a certificate in linguistics.</p></div>
    <div class="abt-m" data-motif="mill"><b>The Netherlands</b><p>A research master's in language at Radboud.</p></div>
    <div class="abt-m" data-motif="robot"><b>Tilburg</b><p>My first robot, teaching Dutch words to Turkish–Dutch children.</p></div>
    <div class="abt-m" data-motif="talk"><b>Koç University</b><p>A PhD on how people talk to robots.</p></div>
    <div class="abt-m next" data-motif="heart"><b>Next</b><p>Still stitching.</p></div>
  </div>
</div>
<div class="abt-patches">
  <a class="abt-patch abt-cloth" href="/projects/talking-to-robots/">See my projects</a>
  <a class="abt-patch abt-cloth" href="/assets/HS_resume_202611.pdf">Resume</a>
  <a class="abt-patch abt-cloth" href="/contact/">Say hello</a>
</div>
</div>
<script>
(function () {
  var root = document.querySelector(".abt");
  if (!root) { return; }
  var NS = "http://www.w3.org/2000/svg";
  var reduce = matchMedia("(prefers-reduced-motion: reduce)").matches;
  var C = { R: "#c8463d", G: "#4f7a4a", L: "#7aa36b", B: "#3c6aa8", Y: "#d9a441", D: "#3a3330", N: "#8a6240", W: "#fbf6ec" };

  var FONT = {
    H: ["X...X", "X...X", "X...X", "XXXXX", "X...X", "X...X", "X...X"],
    A: [".XXX.", "X...X", "X...X", "XXXXX", "X...X", "X...X", "X...X"],
    N: ["X...X", "XX..X", "XX..X", "X.X.X", "X..XX", "X..XX", "X...X"],
    D: ["XXXX.", "X...X", "X...X", "X...X", "X...X", "X...X", "XXXX."],
    E: ["XXXXX", "X....", "X....", "XXXX.", "X....", "X....", "XXXXX"]
  };
  var MOTIFS = {
    tulip: ["...R.R.R...", "..RRRRRRR..", "..RRRRRRR..", "..RRRRRRR..", "...RRRRR...", "....RRR....", ".....G.....", ".LL..G..LL.", "..LL.G.LL..", "...LLGLL...", ".....G.....", ".....G....."],
    mill: ["B.........B", ".B.......B.", "..B.....B..", "...B...B...", "....BYB....", "....NNN....", "...BNNNB...", "..B.NNN.B..", ".B.NNNNN.B.", "...NNNNN...", "..NNNNNNN..", "..NNN.NNN..", "GGGGGGGGGGG"],
    robot: [".....R.....", ".....D.....", "..DDDDDDD..", "..D.....D..", "..D.B.B.D..", "..D.....D..", "..D.RRR.D..", "..DDDDDDD..", "....D.D....", ".BBBBBBBBB.", ".BB.BBB.BB.", ".BBBBBBBBB."],
    talk: [".YYYYYYYY...", "YYYYYYYYYY..", "YYDYYDYYDY..", "YYYYYYYYYY..", ".YYYYYYYY...", "..YY........", ".YY.........", "......BBBBBB", ".....BBBBBBB", ".....BBWBWBB", ".....BBBBBBB", "......BBBBB.", "..........BB"],
    heart: [".RR...RR.", "RRRR.RRRR", "RRRRRRRRR", "RRRRRRRRR", ".RRRRRRR.", "..RRRRR..", "...RRR...", "....R...."]
  };

  function el(n, a) { var e = document.createElementNS(NS, n); for (var k in a) { e.setAttribute(k, a[k]); } return e; }
  function cross(g, x, y, s, col) {
    var p = s * 0.17, w = s * 0.27;
    var st = el("g", { "class": "st" });
    st.appendChild(el("path", { d: "M" + (x + p) + " " + (y + p) + "L" + (x + s - p) + " " + (y + s - p), stroke: col, "stroke-width": w, "stroke-linecap": "round", opacity: ".85" }));
    st.appendChild(el("path", { d: "M" + (x + s - p) + " " + (y + p) + "L" + (x + p) + " " + (y + s - p), stroke: col, "stroke-width": w, "stroke-linecap": "round" }));
    g.appendChild(st);
    return st;
  }
  function draw(rows, s, pad, done) {
    var w = rows[0].length, h = rows.length;
    var svg = el("svg", { viewBox: (-pad) + " " + (-pad) + " " + (w * s + pad * 2) + " " + (h * s + pad * 2), "aria-hidden": "true" });
    var g = el("g", {}); svg.appendChild(g);
    var list = [];
    rows.forEach(function (r, y) {
      for (var x = 0; x < r.length; x++) {
        var ch = r.charAt(x);
        if (ch === "." || !C[ch]) { continue; }
        var stitched = !done || done(x, y, list.length);
        if (stitched) { list.push(cross(g, x * s, y * s, s, C[ch])); }
        else { g.appendChild(el("rect", { x: x * s + s * 0.3, y: y * s + s * 0.3, width: s * 0.4, height: s * 0.4, fill: "none", stroke: C[ch], "stroke-width": s * 0.08, opacity: ".45" })); }
      }
    });
    list.forEach(function (st) { st.style.opacity = reduce ? 1 : 0; });
    svg._st = list;
    return svg;
  }
  function stitchIn(svg, speed) {
    if (reduce) { return; }
    svg._st.forEach(function (st, i) {
      setTimeout(function () { st.style.transition = "opacity .2s"; st.style.opacity = 1; }, i * speed);
    });
  }

  var word = ["H", "A", "N", "D", "E"];
  var rows = [];
  for (var r = 0; r < 7; r++) {
    rows.push(word.map(function (L) { return FONT[L][r].replace(/X/g, "R"); }).join("."));
  }
  rows.push(Array(30).join("."));
  var hrt = [".YY.YY.", "YYYYYYY", ".YYYYY.", "..YYY..", "...Y..."];
  hrt.forEach(function (line) {
    var padL = Math.floor((29 - line.length) / 2);
    rows.push(Array(padL + 1).join(".") + line + Array(29 - padL - line.length + 1).join("."));
  });
  var nameSvg = draw(rows, 9, 4);
  document.getElementById("abt-name").appendChild(nameSvg);

  var motifs = [].slice.call(root.querySelectorAll("[data-motif]"));
  motifs.forEach(function (m) {
    var key = m.getAttribute("data-motif");
    var svg;
    if (key === "heart") {
      svg = draw(MOTIFS.heart, 10, 14, function (x, y) { return y >= 4; });
      var g = el("g", { "class": "abt-needle" });
      g.appendChild(el("path", { d: "M44 46 Q 70 30 78 6", fill: "none", stroke: "#c8463d", "stroke-width": "1.6", "stroke-linecap": "round" }));
      g.appendChild(el("line", { x1: "70", y1: "-2", x2: "96", y2: "-28", stroke: "#9aa0a8", "stroke-width": "3", "stroke-linecap": "round" }));
      g.appendChild(el("ellipse", { cx: "92", cy: "-24", rx: "1.6", ry: "3", transform: "rotate(45 92 -24)", fill: "#f1e7d3" }));
      svg.appendChild(g);
    } else {
      svg = draw(MOTIFS[key], 10, 4);
    }
    m.insertBefore(svg, m.firstChild);
  });

  if ("IntersectionObserver" in window && !reduce) {
    var io = new IntersectionObserver(function (es) {
      es.forEach(function (e) {
        if (!e.isIntersecting) { return; }
        var t = e.target;
        io.unobserve(t);
        if (t.id === "abt-name") { stitchIn(nameSvg, 14); }
        else { setTimeout(function () { stitchIn(t.querySelector("svg"), 22); }, motifs.indexOf(t) * 350); }
      });
    }, { threshold: 0.35 });
    io.observe(document.getElementById("abt-name"));
    motifs.forEach(function (m) { io.observe(m); });
  } else {
    [nameSvg].concat(motifs.map(function (m) { return m.querySelector("svg"); })).forEach(function (s) { s._st.forEach(function (st) { st.style.opacity = 1; }); });
  }
})();
</script>
