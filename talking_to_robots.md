---
title: Talking to Robots
permalink: /projects/talking-to-robots/
layout: page
excerpt: Two controlled experiments on how people talk to machines — reframed as an A/B test and a multivariate test.
comments: false
---
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Bricolage+Grotesque:opsz,wght@12..96,400;12..96,600;12..96,700;12..96,800&family=Instrument+Serif:ital@0;1&family=Space+Mono:wght@400;700&family=Instrument+Sans:wght@400;600&display=swap" rel="stylesheet">
<style>
/* Talking to Robots page. Every rule is scoped to .ttr and every class is prefixed ttr-, so nothing here touches the rest of the site and the theme's own styles cannot leak in. Look: a two-ink risograph zine (fluoro pink + riso blue + yellow) on halftone paper. */
.header:has(+ .page-content .ttr){display:none}
.ttr{--paper:#f5f0e6;--ink:#1d2b6b;--pop:#ff4f9a;--mint:#2f5bff;--sun:#ffd23f;--card:#fffdf7;--muted:#5b6185;--line:rgba(29,43,107,.15);--on-pop:#1d2b6b;--on-mint:#fff;--on-sun:#1d2b6b;--deep:#1d2b6b;--on-deep:#f5f0e6;--c-ok:#2f5bff;--c-bad:#e0352b;
  --f-d:"Bricolage Grotesque",system-ui,-apple-system,"Segoe UI",sans-serif;--f-s:"Instrument Serif",Georgia,serif;--f-m:"Space Mono",ui-monospace,Consolas,monospace;
  position:relative;background-color:var(--paper);background-image:radial-gradient(var(--line) 1.1px,transparent 1.5px);background-size:16px 16px;color:var(--ink);font-family:"Instrument Sans",-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,sans-serif;font-size:18px;line-height:1.6;text-align:left;
  max-width:920px;margin:0 auto;padding:10px 30px 46px;border-radius:10px;overflow:hidden}
body[data-theme="dark"] .ttr{--paper:#11132a;--ink:#f5f0e6;--pop:#ff6aab;--mint:#7b95ff;--card:#1a1d3d;--muted:#a3a8c9;--line:rgba(245,240,230,.13);--on-pop:#11132a;--on-mint:#0b0d20;--deep:#070818;--c-ok:#7b95ff;--c-bad:#ff7a5c}
.ttr *,.ttr *::before,.ttr *::after{box-sizing:border-box}
.ttr p{margin:0 0 14px;padding:0;opacity:1;max-width:680px;color:inherit}
.ttr h1,.ttr h2,.ttr h3{font-family:var(--f-d);color:inherit;margin:0;padding:0;border:0;text-align:left;text-transform:none;letter-spacing:normal}
.ttr h2::before,.ttr h2::after,.ttr h3::before,.ttr h3::after{content:none}
.ttr a{color:inherit}
.ttr a::after{content:none!important}
.ttr button{font-family:inherit}
.ttr-mono{font-family:var(--f-m);font-size:12px;letter-spacing:.08em;text-transform:uppercase}

.ttr-hero{position:relative;padding:44px 0 8px}
.ttr p.ttr-meta{display:inline-block;background:var(--ink);color:var(--paper);padding:4px 10px;margin:0 0 6px!important;max-width:none!important}
.ttr h1.ttr-title{font-weight:800;font-size:clamp(54px,12vw,132px);line-height:.88;letter-spacing:-.045em;margin:18px 0 22px;padding-right:140px;text-shadow:5px 4px 0 var(--pop)}
.ttr-title em{font-family:var(--f-s);font-style:italic;font-weight:400;letter-spacing:-.02em;color:var(--mint);text-shadow:5px 4px 0 var(--sun)}
.ttr-robot{position:absolute;right:4px;top:48px;width:132px;color:var(--ink);filter:drop-shadow(6px 5px 0 var(--pop))}
.ttr-stamp{display:inline-block;border:2px solid var(--ink);padding:7px 14px;transform:rotate(-2.5deg);background:var(--sun);color:var(--on-sun);font-family:var(--f-m);font-size:13px;font-weight:700;box-shadow:4px 4px 0 var(--ink)}
.ttr-ticker{border-top:2px solid var(--ink);border-bottom:2px solid var(--ink);margin:36px -30px 0;overflow:hidden;white-space:nowrap;background:var(--mint)}
.ttr-track{display:inline-block;padding:10px 0;animation:ttr-m 26s linear infinite}
.ttr-tag{display:inline-block;margin:0 24px;color:var(--on-mint);font-family:var(--f-m);font-size:13px;font-weight:700;letter-spacing:.06em;text-transform:uppercase}
.ttr-tag::after{content:"●";margin-left:48px;color:var(--sun)}
@keyframes ttr-m{to{transform:translateX(-50%)}}

.ttr-tldr{margin:38px 0 0;padding:24px 26px;border:2px solid var(--ink);border-radius:8px;background:var(--sun);color:var(--on-sun);box-shadow:8px 8px 0 var(--ink);transform:rotate(-.4deg)}
.ttr-tldr .ttr-mono{font-weight:700;margin-bottom:8px}
.ttr-tldr ol{margin:0;padding:0;list-style:none!important;counter-reset:tl}
.ttr-tldr li{counter-increment:tl;display:flex;gap:14px;margin:10px 0!important;padding:0!important;list-style:none!important;font-family:var(--f-d);font-weight:600;font-size:clamp(17px,2.2vw,20px);line-height:1.35}
.ttr-tldr li::before{content:counter(tl);flex:0 0 30px;height:30px;border-radius:50%;background:var(--pop);color:#1d2b6b;border:2px solid #1d2b6b;font:700 14px/26px var(--f-m);text-align:center;margin:0!important;position:static!important}

.ttr-part{display:flex;align-items:center;gap:14px;flex-wrap:wrap;margin:64px 0 4px;padding-top:16px;border-top:3px solid var(--ink);font-family:var(--f-d);font-weight:800;font-size:clamp(30px,5.4vw,48px);line-height:1;letter-spacing:-.03em}
.ttr-part span{font-family:var(--f-m);font-size:12px;font-weight:700;letter-spacing:.1em;text-transform:uppercase;background:var(--pop);color:var(--on-pop);border:2px solid var(--ink);padding:4px 10px;transform:rotate(-2deg)}

.ttr-block{position:relative;margin:26px 0 0;padding:26px 28px 24px;background:var(--card);border:2px solid var(--ink);border-radius:8px;box-shadow:8px 8px 0 var(--mint)}
.ttr-block:nth-of-type(odd){box-shadow:8px 8px 0 var(--pop)}
.ttr h2.ttr-label{display:flex;align-items:center;gap:14px;font-weight:800;font-size:clamp(28px,4.6vw,42px);line-height:1;letter-spacing:-.03em;margin:0 0 16px}
.ttr-label span{flex:0 0 auto;display:grid;place-items:center;width:52px;height:52px;border-radius:50%;border:2px solid var(--ink);background-color:var(--sun);background-image:radial-gradient(rgba(29,43,107,.35) 1.2px,transparent 1.6px);background-size:6px 6px;color:#1d2b6b;font-family:var(--f-m);font-size:16px;font-weight:700;letter-spacing:0}
.ttr-block p{font-family:var(--f-s);font-weight:400;font-size:clamp(21px,2.8vw,26px);line-height:1.35;max-width:700px}
.ttr-block em{font-style:italic;color:var(--pop)}
.ttr-block strong{font-family:var(--f-d);font-weight:700;font-size:.9em;background:linear-gradient(transparent 58%,var(--sun) 58%);color:inherit}
body[data-theme="dark"] .ttr-block strong{color:var(--ink);background:linear-gradient(transparent 58%,rgba(255,210,63,.45) 58%)}

.ttr-proc{margin:20px 0 4px;background:var(--paper);border:2px solid var(--ink);border-radius:8px;padding:22px 20px 20px;box-shadow:6px 6px 0 var(--sun);text-align:center}
.ttr-ctl{display:flex;flex-wrap:wrap;gap:10px;justify-content:center;margin-bottom:16px}
.ttr-seg{display:inline-flex;border:2px solid var(--ink);border-radius:6px;overflow:hidden;background:var(--card)}
.ttr-seg button{font-weight:600;font-size:13px;border:0;background:none;color:var(--ink);padding:6px 13px;cursor:pointer}
.ttr-seg button.on{background:var(--ink);color:var(--paper)}
.ttr-steps{display:flex;justify-content:center;gap:8px;flex-wrap:wrap;font-family:var(--f-m);font-size:11px;letter-spacing:.06em;text-transform:uppercase;color:var(--muted)}
.ttr-steps span{padding:3px 10px;border:2px solid transparent;transition:.2s}
.ttr-proc[data-step="1"] .ttr-steps span:nth-child(1),.ttr-proc[data-step="2"] .ttr-steps span:nth-child(2),.ttr-proc[data-step="3"] .ttr-steps span:nth-child(3){border-color:var(--ink);background:var(--pop);color:var(--on-pop)}
.ttr-word{font-family:var(--f-d);font-weight:800;font-size:clamp(42px,8vw,66px);line-height:1.05;letter-spacing:-.04em;margin:6px 0 12px;min-height:1.1em}
.ttr-proc[data-step="0"] .ttr-word{font-family:var(--f-s);font-size:clamp(28px,5vw,40px);font-style:italic;font-weight:400;color:var(--muted);letter-spacing:-.01em}
.ttr-meter{height:8px;border:2px solid var(--ink);border-radius:0;background:var(--card);overflow:hidden;max-width:420px;margin:0 auto}
.ttr-fillbar{height:100%;width:100%;background:var(--pop)}
.ttr-clock{font-family:var(--f-m);font-size:12px;letter-spacing:.08em;color:var(--muted);margin:8px 0 0}
.ttr-proc textarea{display:block;width:100%;max-width:560px;margin:0 auto;min-height:78px;resize:none;font-family:"Instrument Sans",sans-serif;font-size:17px;line-height:1.5;color:var(--ink);background:var(--card);border:2px solid var(--ink);border-radius:6px;padding:12px 14px}
.ttr-proc textarea:disabled{opacity:.55}
.ttr-proc textarea:focus{outline:none;box-shadow:4px 4px 0 var(--pop)}
.ttr-screen{position:relative;background:var(--card);border:2px solid var(--ink);border-radius:8px;padding:16px 16px 14px;max-width:560px;margin:16px auto 14px;background-image:radial-gradient(var(--line) 1px,transparent 1.4px);background-size:10px 10px}
.ttr-listener{display:block;width:150px;height:auto;margin:0 auto}
.ttr-proc[data-l="robot"] .lg.hm,.ttr-proc[data-l="human"] .lg.rb{display:none}
.ttr-listener .head,.ttr-listener .body,.ttr-listener .eye,.ttr-listener .ant,.ttr-listener .mouth{transform-box:fill-box;transform-origin:50% 100%}
.ttr-listener .head{animation:ttr-sway 6s ease-in-out infinite}
.ttr-listener .body{animation:ttr-breath 4s ease-in-out infinite}
.ttr-listener .eye{transform-origin:50% 50%;animation:ttr-blink 4.8s infinite}
.ttr-listener .ant{transform-origin:50% 100%;animation:ttr-wob 3s ease-in-out infinite}
.ttr-listener .pupil{transition:transform .12s}
.ttr-listener .hm .mouth,.ttr-proc[data-speak="1"] .hm .smile{display:none}
.ttr-proc[data-speak="1"] .hm .mouth{display:block}
.ttr-proc[data-speak="1"] .ttr-listener .mouth{animation:ttr-talk .2s infinite alternate;transform-origin:50% 50%}
.ttr-proc[data-step="2"] .ttr-listener .head{animation:ttr-listen 2.8s ease-in-out infinite}
.ttr-listener.nod .head{animation:ttr-nod .38s ease-out!important}
.ttr-proc[data-mood="puzzled"] .ttr-listener .head{animation:none;transform:rotate(-8deg)}
.ttr-proc[data-mood="happy"] .ttr-listener .head{animation:ttr-hop .55s ease-out}
@keyframes ttr-sway{0%,100%{transform:translateY(0) rotate(0)}30%{transform:translateY(-2px) rotate(1.6deg)}65%{transform:translateY(1px) rotate(-1.4deg)}}
@keyframes ttr-listen{0%,100%{transform:translateY(0) rotate(-2deg)}50%{transform:translateY(2px) rotate(2.5deg)}}
@keyframes ttr-nod{0%{transform:translateY(0)}40%{transform:translateY(5px)}100%{transform:translateY(0)}}
@keyframes ttr-hop{0%{transform:translateY(0)}35%{transform:translateY(-8px)}100%{transform:translateY(0)}}
@keyframes ttr-breath{0%,100%{transform:scaleY(1)}50%{transform:scaleY(1.025)}}
@keyframes ttr-blink{0%,93%,100%{transform:scaleY(1)}96%{transform:scaleY(.08)}}
@keyframes ttr-wob{0%,100%{transform:rotate(0)}50%{transform:rotate(9deg)}}
@keyframes ttr-talk{from{transform:scaleY(.4)}to{transform:scaleY(1.5)}}
.ttr-bub{position:absolute;top:14px;right:14px;max-width:42%;background:var(--card);border:2px solid var(--ink);border-radius:10px;padding:6px 12px;text-align:left;font-family:var(--f-s);font-style:italic;font-size:18px;line-height:1.25;transition:background .2s;box-shadow:3px 3px 0 var(--ink)}
.ttr-proc[data-mood="happy"] .ttr-bub{background:var(--sun);color:var(--on-sun);font-family:var(--f-d);font-style:normal;font-weight:800}
.ttr-proc[data-mood="puzzled"] .ttr-bub{background:var(--pop);color:var(--on-pop)}
.ttr-go{margin-top:12px;font-family:var(--f-d);font-weight:700;font-size:16px;border:2px solid var(--ink);background:var(--pop);color:var(--on-pop);border-radius:6px;padding:9px 22px;cursor:pointer;box-shadow:4px 4px 0 var(--ink)}
.ttr-go:active{transform:translate(2px,2px);box-shadow:1px 1px 0 var(--ink)}

.ttr-fine{font-family:var(--f-m);font-size:12px;line-height:1.5;color:var(--muted);max-width:640px;margin:8px 0 18px}
.ttr-metric{background:var(--deep);color:var(--on-deep);border:2px solid var(--ink);border-radius:8px;padding:24px;margin:20px 0 0;box-shadow:6px 6px 0 var(--sun)}
.ttr-metric .ttr-mono{color:var(--sun)}
.ttr-say{font-family:var(--f-s);font-size:clamp(26px,4vw,36px);line-height:1.5;margin:12px 0 16px}
.ttr-say button{font:inherit;color:inherit;background:none;border:0;border-bottom:3px dashed #a3a8c9;padding:0 3px;cursor:pointer;transition:.2s}
.ttr-say button.on{background:var(--pop);border-color:var(--pop);color:#1d2b6b}
.ttr-scorebox{display:flex;align-items:center;gap:14px;flex-wrap:wrap}
.ttr-score{font-family:var(--f-d);font-weight:800;font-size:64px;line-height:1;color:var(--sun);min-width:40px}

.ttr-step{display:flex;margin:30px 0;border:2px solid var(--ink);border-radius:8px;background:var(--card);overflow:hidden;box-shadow:8px 8px 0 var(--pop)}
.ttr-step + .ttr-step{box-shadow:8px 8px 0 var(--mint)}
.ttr-num{flex:0 0 70px;display:flex;flex-direction:column;align-items:center;padding-top:18px;background-color:var(--pop);background-image:radial-gradient(rgba(29,43,107,.28) 1.3px,transparent 1.7px);background-size:7px 7px;color:#1d2b6b;border-right:2px solid var(--ink);font-family:var(--f-d);font-weight:800;font-size:44px;line-height:1}
.ttr-num::before{content:"Study";font-family:var(--f-m);font-size:10px;font-weight:700;letter-spacing:.1em;text-transform:uppercase;margin-bottom:6px}
.ttr-step + .ttr-step .ttr-num{background-color:var(--mint);color:#fff;background-image:radial-gradient(rgba(255,255,255,.3) 1.3px,transparent 1.7px)}
.ttr-body{padding:24px 26px 26px;min-width:0;flex:1}
.ttr h3.ttr-steptitle{font-weight:800;font-size:clamp(26px,3.8vw,36px);line-height:1.08;letter-spacing:-.03em;margin:0 0 14px}
.ttr-result{background:var(--paper);border:2px solid var(--ink);border-left:10px solid var(--sun);border-radius:6px;padding:16px 18px;margin:22px 0 0;max-width:680px;font-size:17px}
.ttr-rlabel{display:block;background:var(--ink);color:var(--paper);width:max-content;padding:3px 10px;margin-bottom:10px;font-size:11px;font-weight:700}
.ttr-matrix{display:grid;grid-template-columns:110px 1fr 1fr;gap:8px;margin:18px 0 6px;max-width:580px}
.ttr-cell{border:2px solid var(--ink);border-radius:6px;padding:14px 8px;text-align:center;background:var(--paper);font-family:var(--f-d);font-weight:700;font-size:16px;background-image:repeating-linear-gradient(-45deg,transparent 0 7px,var(--line) 7px 9px)}
.ttr-cell.corner,.ttr-cell.head{border:0;background:none}
.ttr-cell.head{font-family:var(--f-m);font-weight:400;font-size:11px;letter-spacing:.06em;text-transform:uppercase;color:var(--muted);display:flex;align-items:center;justify-content:center;padding:6px}
.ttr-cell.val::before{content:"";display:block;width:40px;height:3px;background:var(--ink);margin:0 auto 8px}
.ttr-caption{font-family:var(--f-m);font-size:12px;line-height:1.5;color:var(--muted);margin-top:8px}
.ttr-sub{display:inline-block;font-weight:700;background:var(--ink);color:var(--paper);padding:3px 10px;margin:28px 0 10px}

.ttr-story{display:grid;grid-template-columns:1fr auto 1fr auto 1fr;gap:8px;align-items:stretch;margin:16px 0 6px}
.ttr-frame{background:var(--paper);border:2px solid var(--ink);border-radius:8px;padding:14px;display:flex;flex-direction:column;gap:8px}
.ttr-frame.hot{background:var(--sun);color:var(--on-sun);box-shadow:5px 5px 0 var(--pop);transform:rotate(-1deg)}
.ttr-fk{font-family:var(--f-m);font-size:11px;letter-spacing:.06em;text-transform:uppercase;opacity:.85}
.ttr-fsay{font-family:var(--f-d);font-weight:700;font-size:16px}
.ttr-fbub{flex:1;border:2px solid currentColor;border-radius:10px;padding:8px 10px;font-family:var(--f-s);font-style:italic;font-size:17px;line-height:1.25}
.ttr-fbub.up{font-family:var(--f-d);font-style:normal;font-weight:800}
.ttr-fbar{height:10px;border:2px solid currentColor;background:transparent;overflow:hidden}
.ttr-fbar i{display:block;height:100%;background:var(--pop)}
.ttr-fnum{font-family:var(--f-d);font-weight:800;font-size:30px;line-height:1}
.ttr-farrow{align-self:center;font-size:24px;font-weight:700}
@media(max-width:700px){.ttr-story{grid-template-columns:1fr}.ttr-farrow{transform:rotate(90deg);justify-self:center}}

.ttr-plot{margin:20px 0 0;max-width:720px}
.ttr-plotsvg{width:100%;height:auto;display:block;overflow:visible}
.ttr-plotsvg .pl-panel{fill:var(--card);stroke:var(--ink);stroke-width:2}
.ttr-plotsvg .pl-band{fill:var(--sun);opacity:.35}
.ttr-plotsvg .pl-grid{stroke:var(--line);stroke-width:1.2}
.ttr-plotsvg .pl-tick{stroke:var(--ink);stroke-width:2}
.ttr-plotsvg .pl-txt{fill:var(--muted);font-family:var(--f-m);font-size:14px}
.ttr-plotsvg .pl-axis{fill:var(--ink);font-family:var(--f-d);font-size:17px;font-weight:700}
.ttr-plotsvg .pl-leg{fill:var(--ink);font-family:"Instrument Sans",sans-serif;font-size:16px}
.ttr-plotsvg .pl-line{stroke:var(--muted);stroke-width:2;fill:none;opacity:.55}
.ttr-plotsvg .pl-err{stroke:var(--muted);stroke-width:2;opacity:.5}
.ttr-plotsvg .pl-dot{stroke:var(--ink);stroke-width:1.5}
.ttr-plotsvg .pl-dot.ok{fill:var(--c-ok)}
.ttr-plotsvg .pl-dot.bad{fill:var(--c-bad)}
.ttr-plotsvg .pl-dot.rep{fill:var(--sun)}
.ttr-plotsvg .pl-val{fill:var(--ink);font-family:var(--f-d);font-weight:800;font-size:26px}
.ttr-plotsvg .pl-bar{stroke:var(--ink);stroke-width:2.5}
.ttr-plotsvg .pl-bar.h{fill:var(--mint)}
.ttr-plotsvg .pl-bar.r{fill:var(--pop)}
.ttr-plotsvg .pl-shadow{fill:var(--ink);opacity:.9}
.ttr-plotsvg .pl-delta{fill:var(--ink);font-family:var(--f-m);font-weight:700;font-size:15px}
.ttr-plotsvg circle{transition:r .15s}
.ttr-plotsvg .pl-dot:hover{r:10}

.ttr-biz{display:grid;grid-template-columns:1fr 1fr;gap:18px;margin:26px 0 0}
.ttr-bcard{background:var(--card);border:2px solid var(--ink);border-radius:8px;padding:20px 22px 6px;box-shadow:6px 6px 0 var(--mint)}
.ttr-bcard:nth-child(4n+1),.ttr-bcard:nth-child(4n){box-shadow:6px 6px 0 var(--pop)}
.ttr-bstat{display:inline-block;font-family:var(--f-d);font-weight:800;font-size:clamp(40px,6vw,56px);line-height:1;letter-spacing:-.04em;color:var(--pop);text-shadow:3px 3px 0 var(--sun);margin-bottom:10px}
.ttr-bcard:nth-child(even) .ttr-bstat{color:var(--mint)}
.ttr-btitle{font-family:var(--f-d);font-weight:800;font-size:clamp(22px,2.8vw,27px);line-height:1.1;letter-spacing:-.02em;margin-bottom:6px}
.ttr-bcard p{font-size:16px;line-height:1.5;color:var(--muted)}
@media(max-width:700px){.ttr-biz{grid-template-columns:1fr}}
.ttr-insight{margin:40px 0 10px;background-color:var(--mint);background-image:radial-gradient(rgba(255,255,255,.18) 1.3px,transparent 1.7px);background-size:9px 9px;color:var(--on-mint);border:2px solid var(--ink);border-radius:8px;padding:34px 30px;box-shadow:10px 10px 0 var(--pop)}
.ttr-insight .ttr-mono{display:inline-block;background:var(--sun);color:var(--on-sun);font-weight:700;padding:3px 10px;margin-bottom:14px}
.ttr-insight p{font-family:var(--f-d);font-weight:700;font-size:clamp(20px,2.8vw,27px);line-height:1.3;letter-spacing:-.015em;max-width:760px;margin:0}
.ttr-actions{margin:36px 0 6px}
.ttr a.ttr-btn{display:inline-block;text-decoration:none;font-family:var(--f-d);font-weight:700;font-size:17px;padding:14px 24px;border:2px solid var(--ink);border-radius:6px;background:var(--sun);color:var(--on-sun);box-shadow:5px 5px 0 var(--ink);transition:transform .12s,box-shadow .12s}
.ttr a.ttr-btn:hover{transform:translate(-2px,-2px);box-shadow:7px 7px 0 var(--ink)}
@media(max-width:600px){.ttr-bub{max-width:52%;font-size:15px}.ttr{padding:6px 16px 32px;font-size:16px}.ttr-ticker{margin-inline:-16px}.ttr-robot{display:none}.ttr h1.ttr-title{padding-right:0}.ttr-block{padding:20px 18px}.ttr-label span{width:42px;height:42px;font-size:14px}.ttr-num{flex-basis:50px;font-size:32px}.ttr-num::before{font-size:8px}.ttr-body{padding:18px 16px}.ttr-matrix{grid-template-columns:76px 1fr 1fr}.ttr-insight{padding:26px 20px}.ttr-tldr{padding:20px 18px}}
@media(prefers-reduced-motion:reduce){.ttr-track,.ttr-listener *{animation:none!important}}
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
  <p class="ttr-mono ttr-meta">PhD research on how people talk to machines &middot; Koç University &middot; 2020–2026</p>
  <h1 class="ttr-title">Talking to <em>Robots.</em></h1>
  <div class="ttr-stamp">★ HRI '26 · Honorable Mention</div>
</div>
<div class="ttr-ticker" aria-label="Skills"><div class="ttr-track">
  <span class="ttr-tag">A/B Testing</span><span class="ttr-tag">Multivariate Testing</span><span class="ttr-tag">Behavioral Analytics</span><span class="ttr-tag">R</span><span class="ttr-tag">Experimental Design</span>
  <span class="ttr-tag" aria-hidden="true">A/B Testing</span><span class="ttr-tag" aria-hidden="true">Multivariate Testing</span><span class="ttr-tag" aria-hidden="true">Behavioral Analytics</span><span class="ttr-tag" aria-hidden="true">R</span><span class="ttr-tag" aria-hidden="true">Experimental Design</span>
</div></div>
<div class="ttr-tldr">
  <div class="ttr-mono">The short version</div>
  <ol>
    <li>People give a robot more detail than a human, even when the robot keeps getting it right.</li>
    <li>Robot confidence claims and specific praise change nothing.</li>
    <li>What does change it: the robot visibly failing to understand, and only on the very next attempt.</li>
  </ol>
</div>
<div class="ttr-part"><span>Part one</span>The setup</div>
<div class="ttr-block">
  <h2 class="ttr-label"><span>01</span>The question</h2>
  <p>How much should a robot, chatbot, or voice assistant signal that it understands you? I tested how people change what they say based on those signals.</p>
  <p>A robot is a useful test case because it is neither predictable like a person nor simple like a button. People can't lean on social intuition about what it understands, so we can see which signals actually move behavior.</p>
</div>
<div class="ttr-block">
  <h2 class="ttr-label"><span>02</span>The game</h2>
  <p>Speakers had seven seconds to describe a word without saying it, while a human or a robot listener tried to guess. Both listeners behaved identically, so the only thing that changed was <em>who</em> was listening. Play a round below: you are the speaker.</p>
  <div class="ttr-proc" id="ttr-proc" data-l="robot" data-g="ok" data-step="0">
    <div class="ttr-ctl">
      <div class="ttr-seg" data-k="l" role="group" aria-label="Who is listening">
        <button type="button" data-v="robot" class="on" aria-pressed="true">Robot listener</button>
        <button type="button" data-v="human" aria-pressed="false">Human listener</button>
      </div>
      <div class="ttr-seg" data-k="g" role="group" aria-label="What the listener does">
        <button type="button" data-v="ok" class="on" aria-pressed="true">Guesses right</button>
        <button type="button" data-v="bad" aria-pressed="false">Gets it wrong</button>
      </div>
    </div>
    <div class="ttr-steps" aria-hidden="true"><span>1 · Word appears</span><span>2 · You describe it</span><span>3 · Listener guesses</span></div>
    <div class="ttr-screen">
      <svg class="ttr-listener" id="ttr-listener" viewBox="0 0 160 150" aria-hidden="true">
        <g class="lg rb">
          <g class="body"><path d="M24 150C24 118 50 106 80 106C110 106 136 118 136 150Z" fill="var(--mint)" stroke="var(--ink)" stroke-width="4"/><circle cx="80" cy="132" r="9" fill="var(--paper)" stroke="var(--ink)" stroke-width="3.5"/></g>
          <g class="head">
            <line x1="80" y1="10" x2="80" y2="24" stroke="var(--ink)" stroke-width="4" stroke-linecap="round"/>
            <circle class="ant" cx="80" cy="8" r="5.5" fill="var(--pop)"/>
            <rect x="34" y="22" width="92" height="72" rx="26" fill="var(--paper)" stroke="var(--ink)" stroke-width="4"/>
            <g class="eye"><circle cx="60" cy="54" r="12" fill="var(--card)" stroke="var(--ink)" stroke-width="3"/><circle class="pupil" cx="60" cy="54" r="5.5" fill="var(--ink)"/></g>
            <g class="eye"><circle cx="100" cy="54" r="12" fill="var(--card)" stroke="var(--ink)" stroke-width="3"/><circle class="pupil" cx="100" cy="54" r="5.5" fill="var(--ink)"/></g>
            <ellipse class="mouth" cx="80" cy="78" rx="6" ry="4.5" fill="var(--pop)"/>
          </g>
        </g>
        <g class="lg hm">
          <g class="body"><path d="M24 150C24 118 50 106 80 106C110 106 136 118 136 150Z" fill="var(--pop)" stroke="var(--ink)" stroke-width="4"/></g>
          <g class="head">
            <path d="M36 64C28 8 132 8 124 64L126 104C126 114 112 114 112 104L112 74L48 74L48 104C48 114 34 114 34 104Z" fill="#7a4a2b"/>
            <circle cx="80" cy="60" r="35" fill="var(--paper)" stroke="var(--ink)" stroke-width="4"/>
            <path d="M42 56C42 20 118 18 118 56C112 44 100 36 86 34C84 42 66 48 42 56Z" fill="#7a4a2b"/>
            <circle cx="80" cy="14" r="9" fill="#7a4a2b"/>
            <g class="eye"><circle cx="64" cy="62" r="7" fill="var(--card)" stroke="var(--ink)" stroke-width="2.5"/><circle class="pupil" cx="64" cy="62" r="3.4" fill="var(--ink)"/></g>
            <g class="eye"><circle cx="96" cy="62" r="7" fill="var(--card)" stroke="var(--ink)" stroke-width="2.5"/><circle class="pupil" cx="96" cy="62" r="3.4" fill="var(--ink)"/></g>
            <path class="smile" d="M68 82Q80 90 92 82" fill="none" stroke="var(--ink)" stroke-width="3.5" stroke-linecap="round"/>
            <ellipse class="mouth" cx="80" cy="84" rx="7" ry="5" fill="var(--ink)"/>
          </g>
        </g>
      </svg>
      <div class="ttr-bub" id="ttr-said">(Listening)</div>
      <div class="ttr-word" id="ttr-word" aria-live="polite">You are the speaker</div>
      <div class="ttr-meter"><div class="ttr-fillbar" id="ttr-fill"></div></div>
      <div class="ttr-clock" id="ttr-clock">7.0 s</div>
    </div>
    <textarea id="ttr-text" rows="2" maxlength="220" placeholder="Describe the word. Don't say it." aria-label="Your description" disabled></textarea>
    <button class="ttr-go" id="ttr-go" type="button">Start</button>
  </div>
</div>
<div class="ttr-block">
  <h2 class="ttr-label"><span>03</span>The measure</h2>
  <p>To compare descriptions, I built a metric, <strong>semantic detail density</strong>: the number of separate, meaningful pieces of information in a description. <em>"A large vehicle used to carry stuff"</em> scores three.</p>
  <div class="ttr-metric">
    <div class="ttr-mono">Try it · tap each detail</div>
    <div class="ttr-say">“a <button type="button" data-d>large</button> <button type="button" data-d>vehicle</button> <button type="button" data-d>used to carry stuff</button>”</div>
    <div class="ttr-scorebox"><div class="ttr-score" id="ttr-score">0</div><div class="ttr-mono">points of detail</div></div>
  </div>
</div>
<div class="ttr-part"><span>Part two</span>The experiments</div>
<div class="ttr-step">
  <div class="ttr-num">1</div>
  <div class="ttr-body">
    <h3 class="ttr-steptitle">Does the listener change what people say?</h3>
    <p>First, the baseline: the same game, with a human or a robot on the other side. Everything else stayed the same.</p>
    <div class="ttr-plot">
      <svg class="ttr-plotsvg" viewBox="0 0 880 250" role="img" aria-label="Mean detail by listener: human listener 1.98, robot listener 2.23."><rect class="pl-panel" x="170" y="14" width="640" height="172"/><line class="pl-grid" x1="170.0" x2="170.0" y1="14" y2="186"/><line class="pl-tick" x1="170.0" x2="170.0" y1="186" y2="192"/><text class="pl-txt" x="170.0" y="210" text-anchor="middle">0.0</text><line class="pl-grid" x1="276.7" x2="276.7" y1="14" y2="186"/><line class="pl-tick" x1="276.7" x2="276.7" y1="186" y2="192"/><text class="pl-txt" x="276.7" y="210" text-anchor="middle">0.5</text><line class="pl-grid" x1="383.3" x2="383.3" y1="14" y2="186"/><line class="pl-tick" x1="383.3" x2="383.3" y1="186" y2="192"/><text class="pl-txt" x="383.3" y="210" text-anchor="middle">1.0</text><line class="pl-grid" x1="490.0" x2="490.0" y1="14" y2="186"/><line class="pl-tick" x1="490.0" x2="490.0" y1="186" y2="192"/><text class="pl-txt" x="490.0" y="210" text-anchor="middle">1.5</text><line class="pl-grid" x1="596.7" x2="596.7" y1="14" y2="186"/><line class="pl-tick" x1="596.7" x2="596.7" y1="186" y2="192"/><text class="pl-txt" x="596.7" y="210" text-anchor="middle">2.0</text><line class="pl-grid" x1="703.3" x2="703.3" y1="14" y2="186"/><line class="pl-tick" x1="703.3" x2="703.3" y1="186" y2="192"/><text class="pl-txt" x="703.3" y="210" text-anchor="middle">2.5</text><line class="pl-grid" x1="810.0" x2="810.0" y1="14" y2="186"/><line class="pl-tick" x1="810.0" x2="810.0" y1="186" y2="192"/><text class="pl-txt" x="810.0" y="210" text-anchor="middle">3.0</text><rect class="pl-shadow" x="175.0" y="36.4" width="423.0" height="58"/><rect class="pl-bar h" x="170.0" y="31.4" width="423.0" height="58"><title>Human listener: 1.98</title></rect><text class="pl-val" x="607.0" y="69.4">1.98</text><text class="pl-axis" x="156" y="66.4" text-anchor="end">Human listener</text><rect class="pl-shadow" x="175.0" y="115.6" width="475.1" height="58"/><rect class="pl-bar r" x="170.0" y="110.6" width="475.1" height="58"><title>Robot listener: 2.23</title></rect><text class="pl-val" x="659.1" y="148.6">2.23</text><text class="pl-axis" x="156" y="145.6" text-anchor="end">Robot listener</text><text class="pl-axis" x="490" y="242" text-anchor="middle">Mean detail</text></svg>
    </div>
    <div class="ttr-result">
      <span class="ttr-mono ttr-rlabel">Result</span>
      Yes. People gave the robot more detail than the human (2.23 vs 1.98 on average), in every error-trajectory condition, even after the robot got several answers right in a row. This work was published at ACM/IEEE HRI '26 with an Honorable Mention.
    </div>
  </div>
</div>
<div class="ttr-step">
  <div class="ttr-num">2</div>
  <div class="ttr-body">
    <h3 class="ttr-steptitle">Which robot signals change behavior?</h3>
    <p>Since people gave the robot more detail, I asked whether the robot can influence how much they say. I tested two kinds of signal.</p>
    <div class="ttr-mono ttr-sub">Test A · Two signals, crossed</div>
    <p>An upfront competence claim, and specific positive feedback after a correct guess, each present or absent.</p>
    <div class="ttr-matrix">
      <div class="ttr-cell corner"></div>
      <div class="ttr-cell head">No competence claim</div>
      <div class="ttr-cell head">Competence claim</div>
      <div class="ttr-cell head">Generic feedback</div>
      <div class="ttr-cell val">No effect</div>
      <div class="ttr-cell val">No effect</div>
      <div class="ttr-cell head">Specific feedback</div>
      <div class="ttr-cell val">No effect</div>
      <div class="ttr-cell val">No effect</div>
    </div>
    <div class="ttr-caption">None of the four combinations moved the metric.</div>
    <div class="ttr-mono ttr-sub">Test B · The robot fails</div>
    <p>On some rounds the robot said it couldn't find the answer and asked for another description. This is where behavior moved.</p>
    <div class="ttr-story">
      <div class="ttr-frame">
        <div class="ttr-fk">Trial 4 · the robot errs</div>
        <div class="ttr-fsay">You describe the word.</div>
        <div class="ttr-fbub">“Hmm, I couldn't find it. Could you describe it again?”</div>
        <div class="ttr-fbar"><i style="width:81.7%"></i></div><div class="ttr-fnum">2.45</div>
      </div>
      <div class="ttr-farrow" aria-hidden="true">→</div>
      <div class="ttr-frame hot">
        <div class="ttr-fk">The retry</div>
        <div class="ttr-fsay">You add detail.</div>
        <div class="ttr-fbub up">+0.20 more detail</div>
        <div class="ttr-fbar"><i style="width:88.3%"></i></div><div class="ttr-fnum">2.65</div>
      </div>
      <div class="ttr-farrow" aria-hidden="true">→</div>
      <div class="ttr-frame">
        <div class="ttr-fk">Trial 5 · robot is right</div>
        <div class="ttr-fsay">You relax back.</div>
        <div class="ttr-fbub">“Truck!”</div>
        <div class="ttr-fbar"><i style="width:77%"></i></div><div class="ttr-fnum">2.31</div>
      </div>
    </div>
    <div class="ttr-fine">Mean semantic detail density across speakers, trial 4 shown. The same rise happened at trials 9, 11 and 15. The full picture is below.</div>
    <div class="ttr-plot">
      <svg class="ttr-plotsvg" viewBox="0 0 880 420" role="img" aria-label="Mean semantic detail density by trial. On the four trials where the robot erred (4, 9, 11 and 15), the repair attempt is higher than the incorrect trial it followed, while correct trials stay flat around 2.3 to 2.5."><rect class="pl-panel" x="74" y="64" width="790" height="294"/><rect class="pl-band" x="229.5" y="64" width="34.6" height="294"/><rect class="pl-band" x="476.4" y="64" width="34.6" height="294"/><rect class="pl-band" x="575.2" y="64" width="34.6" height="294"/><rect class="pl-band" x="772.7" y="64" width="34.6" height="294"/><line class="pl-grid" x1="74" x2="864" y1="333.5" y2="333.5"/><line class="pl-tick" x1="68" x2="74" y1="333.5" y2="333.5"/><text class="pl-txt" x="64" y="338.5" text-anchor="end">2.00</text><line class="pl-grid" x1="74" x2="864" y1="272.2" y2="272.2"/><line class="pl-tick" x1="68" x2="74" y1="272.2" y2="272.2"/><text class="pl-txt" x="64" y="277.2" text-anchor="end">2.25</text><line class="pl-grid" x1="74" x2="864" y1="211.0" y2="211.0"/><line class="pl-tick" x1="68" x2="74" y1="211.0" y2="211.0"/><text class="pl-txt" x="64" y="216.0" text-anchor="end">2.50</text><line class="pl-grid" x1="74" x2="864" y1="149.8" y2="149.8"/><line class="pl-tick" x1="68" x2="74" y1="149.8" y2="149.8"/><text class="pl-txt" x="64" y="154.8" text-anchor="end">2.75</text><line class="pl-grid" x1="74" x2="864" y1="88.5" y2="88.5"/><line class="pl-tick" x1="68" x2="74" y1="88.5" y2="88.5"/><text class="pl-txt" x="64" y="93.5" text-anchor="end">3.00</text><line class="pl-tick" x1="98.7" x2="98.7" y1="358" y2="364"/><text class="pl-txt" x="98.7" y="382" text-anchor="middle">1</text><line class="pl-tick" x1="148.1" x2="148.1" y1="358" y2="364"/><text class="pl-txt" x="148.1" y="382" text-anchor="middle">2</text><line class="pl-tick" x1="197.4" x2="197.4" y1="358" y2="364"/><text class="pl-txt" x="197.4" y="382" text-anchor="middle">3</text><line class="pl-tick" x1="246.8" x2="246.8" y1="358" y2="364"/><text class="pl-txt" x="246.8" y="382" text-anchor="middle">4</text><line class="pl-tick" x1="296.2" x2="296.2" y1="358" y2="364"/><text class="pl-txt" x="296.2" y="382" text-anchor="middle">5</text><line class="pl-tick" x1="345.6" x2="345.6" y1="358" y2="364"/><text class="pl-txt" x="345.6" y="382" text-anchor="middle">6</text><line class="pl-tick" x1="394.9" x2="394.9" y1="358" y2="364"/><text class="pl-txt" x="394.9" y="382" text-anchor="middle">7</text><line class="pl-tick" x1="444.3" x2="444.3" y1="358" y2="364"/><text class="pl-txt" x="444.3" y="382" text-anchor="middle">8</text><line class="pl-tick" x1="493.7" x2="493.7" y1="358" y2="364"/><text class="pl-txt" x="493.7" y="382" text-anchor="middle">9</text><line class="pl-tick" x1="543.1" x2="543.1" y1="358" y2="364"/><text class="pl-txt" x="543.1" y="382" text-anchor="middle">10</text><line class="pl-tick" x1="592.4" x2="592.4" y1="358" y2="364"/><text class="pl-txt" x="592.4" y="382" text-anchor="middle">11</text><line class="pl-tick" x1="641.8" x2="641.8" y1="358" y2="364"/><text class="pl-txt" x="641.8" y="382" text-anchor="middle">12</text><line class="pl-tick" x1="691.2" x2="691.2" y1="358" y2="364"/><text class="pl-txt" x="691.2" y="382" text-anchor="middle">13</text><line class="pl-tick" x1="740.6" x2="740.6" y1="358" y2="364"/><text class="pl-txt" x="740.6" y="382" text-anchor="middle">14</text><line class="pl-tick" x1="789.9" x2="789.9" y1="358" y2="364"/><text class="pl-txt" x="789.9" y="382" text-anchor="middle">15</text><line class="pl-tick" x1="839.3" x2="839.3" y1="358" y2="364"/><text class="pl-txt" x="839.3" y="382" text-anchor="middle">16</text><path class="pl-line" d="M148.1 240.4L197.4 220.8M197.4 220.8L246.8 223.2M246.8 174.3L296.2 257.5M296.2 257.5L345.6 198.8M345.6 198.8L394.9 211.0M394.9 211.0L444.3 237.9M444.3 237.9L493.7 225.7M493.7 157.1L543.1 240.4M543.1 240.4L592.4 211.0M592.4 149.8L641.8 282.1M641.8 282.1L691.2 237.9M691.2 237.9L740.6 220.8M740.6 220.8L789.9 250.2M789.9 162.0L839.3 240.4M98.7 223.2L148.1 240.4"/><line class="pl-err" x1="98.7" x2="98.7" y1="251.2" y2="195.3"/><line class="pl-err" x1="148.1" x2="148.1" y1="269.8" y2="211.0"/><line class="pl-err" x1="197.4" x2="197.4" y1="249.7" y2="191.9"/><line class="pl-err" x1="246.8" x2="246.8" y1="252.9" y2="193.6"/><line class="pl-err" x1="246.8" x2="246.8" y1="206.8" y2="141.7"/><line class="pl-err" x1="296.2" x2="296.2" y1="282.1" y2="233.0"/><line class="pl-err" x1="345.6" x2="345.6" y1="230.4" y2="167.1"/><line class="pl-err" x1="394.9" x2="394.9" y1="241.1" y2="180.9"/><line class="pl-err" x1="444.3" x2="444.3" y1="266.1" y2="209.8"/><line class="pl-err" x1="493.7" x2="493.7" y1="256.8" y2="194.6"/><line class="pl-err" x1="493.7" x2="493.7" y1="189.7" y2="124.5"/><line class="pl-err" x1="543.1" x2="543.1" y1="269.6" y2="211.2"/><line class="pl-err" x1="592.4" x2="592.4" y1="241.6" y2="180.4"/><line class="pl-err" x1="592.4" x2="592.4" y1="181.4" y2="118.1"/><line class="pl-err" x1="641.8" x2="641.8" y1="310.5" y2="253.6"/><line class="pl-err" x1="691.2" x2="691.2" y1="268.3" y2="207.6"/><line class="pl-err" x1="740.6" x2="740.6" y1="247.0" y2="194.6"/><line class="pl-err" x1="789.9" x2="789.9" y1="278.4" y2="222.0"/><line class="pl-err" x1="789.9" x2="789.9" y1="197.3" y2="126.7"/><line class="pl-err" x1="839.3" x2="839.3" y1="271.3" y2="209.5"/><circle class="pl-dot ok" cx="98.7" cy="223.2" r="7.5"><title>Trial 1 · Correct: 2.45 (SE 0.114)</title></circle><circle class="pl-dot ok" cx="148.1" cy="240.4" r="7.5"><title>Trial 2 · Correct: 2.38 (SE 0.120)</title></circle><circle class="pl-dot ok" cx="197.4" cy="220.8" r="7.5"><title>Trial 3 · Correct: 2.46 (SE 0.118)</title></circle><circle class="pl-dot bad" cx="246.8" cy="223.2" r="7.5"><title>Trial 4 · Incorrect: 2.45 (SE 0.121)</title></circle><circle class="pl-dot rep" cx="246.8" cy="174.3" r="7.5"><title>Trial 4 · Repair: 2.65 (SE 0.133)</title></circle><circle class="pl-dot ok" cx="296.2" cy="257.5" r="7.5"><title>Trial 5 · Correct: 2.31 (SE 0.100)</title></circle><circle class="pl-dot ok" cx="345.6" cy="198.8" r="7.5"><title>Trial 6 · Correct: 2.55 (SE 0.129)</title></circle><circle class="pl-dot ok" cx="394.9" cy="211.0" r="7.5"><title>Trial 7 · Correct: 2.50 (SE 0.123)</title></circle><circle class="pl-dot ok" cx="444.3" cy="237.9" r="7.5"><title>Trial 8 · Correct: 2.39 (SE 0.115)</title></circle><circle class="pl-dot bad" cx="493.7" cy="225.7" r="7.5"><title>Trial 9 · Incorrect: 2.44 (SE 0.127)</title></circle><circle class="pl-dot rep" cx="493.7" cy="157.1" r="7.5"><title>Trial 9 · Repair: 2.72 (SE 0.133)</title></circle><circle class="pl-dot ok" cx="543.1" cy="240.4" r="7.5"><title>Trial 10 · Correct: 2.38 (SE 0.119)</title></circle><circle class="pl-dot bad" cx="592.4" cy="211.0" r="7.5"><title>Trial 11 · Incorrect: 2.50 (SE 0.125)</title></circle><circle class="pl-dot rep" cx="592.4" cy="149.8" r="7.5"><title>Trial 11 · Repair: 2.75 (SE 0.129)</title></circle><circle class="pl-dot ok" cx="641.8" cy="282.1" r="7.5"><title>Trial 12 · Correct: 2.21 (SE 0.116)</title></circle><circle class="pl-dot ok" cx="691.2" cy="237.9" r="7.5"><title>Trial 13 · Correct: 2.39 (SE 0.124)</title></circle><circle class="pl-dot ok" cx="740.6" cy="220.8" r="7.5"><title>Trial 14 · Correct: 2.46 (SE 0.107)</title></circle><circle class="pl-dot bad" cx="789.9" cy="250.2" r="7.5"><title>Trial 15 · Incorrect: 2.34 (SE 0.115)</title></circle><circle class="pl-dot rep" cx="789.9" cy="162.0" r="7.5"><title>Trial 15 · Repair: 2.70 (SE 0.144)</title></circle><circle class="pl-dot ok" cx="839.3" cy="240.4" r="7.5"><title>Trial 16 · Correct: 2.38 (SE 0.126)</title></circle><text class="pl-axis" x="469" y="408" text-anchor="middle">Trial (within-block order)</text><text class="pl-axis" transform="translate(18 211) rotate(-90)" text-anchor="middle">Mean semantic detail density</text><circle class="pl-dot ok" cx="270" cy="28" r="7.5"/><text class="pl-leg" x="284" y="34">Correct</text><circle class="pl-dot bad" cx="390" cy="28" r="7.5"/><text class="pl-leg" x="404" y="34">Incorrect</text><circle class="pl-dot rep" cx="510" cy="28" r="7.5"/><text class="pl-leg" x="524" y="34">Repair</text><text class="pl-delta" x="246.8" y="132.7" text-anchor="middle">+0.20</text><text class="pl-delta" x="493.7" y="115.5" text-anchor="middle">+0.28</text><text class="pl-delta" x="592.4" y="109.1" text-anchor="middle">+0.25</text><text class="pl-delta" x="789.9" y="117.7" text-anchor="middle">+0.36</text></svg>
      <div class="ttr-fine" style="margin-bottom:0">Shaded columns mark trials where the robot erred. Labels show the rise on the retry.</div>
    </div>
    <div class="ttr-result">
      <span class="ttr-mono ttr-rlabel">Result</span>
      Neither the competence claim nor the specific feedback changed anything, alone or together. But when the robot said it didn't understand and asked for a retry, people added detail on that attempt only (repair means 2.65 to 2.75, against 2.34 to 2.50 for the error trial just before), then went back to normal.
    </div>
  </div>
</div>
<div class="ttr-part"><span>Part three</span>What it means for products</div>
<div class="ttr-biz">
  <div class="ttr-bcard"><div class="ttr-bstat">+12%</div><div class="ttr-btitle">Users over-explain to bots.</div><p>Expect wordier input. Success won't shrink it.</p></div>
  <div class="ttr-bcard"><div class="ttr-bstat">0 / 4</div><div class="ttr-btitle">Self-promotion doesn't work.</div><p>Competence claims and praise changed nothing.</p></div>
  <div class="ttr-bcard"><div class="ttr-bstat">4 / 4</div><div class="ttr-btitle">Failure gets better input.</div><p>A clear “I didn't get that” raised detail on every retry.</p></div>
  <div class="ttr-bcard"><div class="ttr-bstat">1 turn</div><div class="ttr-btitle">One fix doesn't last.</div><p>So show what the system understood, every turn.</p></div>
</div>
<div class="ttr-insight">
  <div class="ttr-mono">The takeaway</div>
  <p>Who users think they are talking to sets how much they say. What moved it was not what the system claimed about itself, but clear evidence that it had not understood.</p>
</div>
<div class="ttr-actions">
  <a class="ttr-btn" href="/academia/">Full write-ups &amp; citations</a>
</div>
</div>
<script>
(function () {
  var root = document.querySelector(".ttr");
  if (!root) { return; }
  var robot = root.querySelector(".ttr-robot");
  var pupils = [].slice.call(root.querySelectorAll(".ttr-pupil"));
  addEventListener("pointermove", function (e) {
    var bb = robot.getBoundingClientRect();
    if (!bb.width) { return; }
    var a = Math.atan2(e.clientY - (bb.top + bb.height / 2), e.clientX - (bb.left + bb.width / 2));
    pupils.forEach(function (p) {
      p.style.transform = "translate(" + Math.cos(a) * 5 + "px," + Math.sin(a) * 5 + "px)";
    });
  });
  var proc = document.getElementById("ttr-proc");
  var go = document.getElementById("ttr-go");
  var wordEl = document.getElementById("ttr-word");
  var fill = document.getElementById("ttr-fill");
  var clock = document.getElementById("ttr-clock");
  var box = document.getElementById("ttr-text");
  var said = document.getElementById("ttr-said");
  var pool = ["truck", "umbrella", "kettle", "bicycle"];
  var wi = -1;
  var word = "";
  var round = 1;
  var raf = 0;
  var tm = 0;
  var busy = false;
  function reset() {
    cancelAnimationFrame(raf);
    clearTimeout(tm);
    busy = false;
  }
  function counting() {
    var start = Date.now();
    function tick() {
      var left = Math.max(0, 7000 - (Date.now() - start));
      fill.style.width = (left / 7000 * 100) + "%";
      clock.textContent = (left / 1000).toFixed(1) + " s";
      if (left > 0) { raf = requestAnimationFrame(tick); } else { finish(); }
    }
    tick();
  }
  function begin(repair) {
    reset();
    busy = true;
    proc.setAttribute("data-step", "1");
    go.disabled = true;
    go.style.opacity = ".5";
    said.textContent = "(Listening)";
    proc.removeAttribute("data-mood");
    proc.removeAttribute("data-speak");
    wordEl.textContent = word;
    fill.style.width = "100%";
    clock.textContent = "7.0 s";
    box.value = "";
    tm = setTimeout(function () {
      proc.setAttribute("data-step", "2");
      box.disabled = false;
      box.focus();
      counting();
    }, 800);
  }
  function finish() {
    box.disabled = true;
    proc.setAttribute("data-step", "3");
    var wrong = proc.getAttribute("data-g") === "bad" && round === 1;
    tm = setTimeout(function () {
      busy = false;
      go.disabled = false;
      go.style.opacity = "1";
      proc.setAttribute("data-speak", "1");
      setTimeout(function () { proc.removeAttribute("data-speak"); }, 1300);
      proc.setAttribute("data-mood", wrong ? "puzzled" : "happy");
      if (wrong) {
        said.textContent = "“Hmm, I couldn't find it. Could you describe it again?”";
        go.textContent = "Describe it again";
        round = 2;
      } else {
        said.textContent = "“" + word.charAt(0).toUpperCase() + word.slice(1) + "!”";
        go.textContent = "Try another word";
        round = 1;
      }
    }, 700);
  }
  var av = document.getElementById("ttr-listener");
  var nodTimer = 0;
  box.addEventListener("input", function () {
    av.classList.remove("nod");
    void av.getBoundingClientRect();
    av.classList.add("nod");
    clearTimeout(nodTimer);
    nodTimer = setTimeout(function () { av.classList.remove("nod"); }, 400);
  });
  var eyesAll = [].slice.call(av.querySelectorAll(".pupil"));
  function gaze(x, y) {
    eyesAll.forEach(function (p) { p.style.transform = "translate(" + x + "px," + y + "px)"; });
  }
  function glance() {
    var r = Math.random();
    var spots = [[-3.5, -1], [3.5, -1], [-3, 2], [3, 2], [0, -3], [2, 0]];
    var d = spots[Math.floor(Math.random() * spots.length)];
    if (r < 0.25) { gaze(((Math.random() - .5) * 1.2).toFixed(1), ((Math.random() - .5) * 1.2).toFixed(1)); }
    else { gaze(d[0], d[1]); }
    setTimeout(function () { gaze(0, 0); }, 500 + Math.random() * 900);
    setTimeout(glance, 2200 + Math.random() * 3800);
  }
  gaze(0, 0);
  setTimeout(glance, 2500);
  go.addEventListener("click", function () {
    if (busy) { return; }
    if (round === 1) { wi = (wi + 1) % pool.length; word = pool[wi]; }
    go.textContent = "Start";
    begin();
  });
  [].forEach.call(proc.querySelectorAll(".ttr-seg"), function (seg) {
    var key = seg.getAttribute("data-k");
    [].forEach.call(seg.querySelectorAll("button"), function (b) {
      b.addEventListener("click", function () {
        proc.setAttribute("data-" + key, b.getAttribute("data-v"));
        [].forEach.call(seg.querySelectorAll("button"), function (o) {
          var on = o === b;
          o.classList.toggle("on", on);
          o.setAttribute("aria-pressed", on ? "true" : "false");
        });
      });
    });
  });
  var score = document.getElementById("ttr-score");
  [].forEach.call(root.querySelectorAll("[data-d]"), function (el) {
    el.addEventListener("click", function () {
      el.classList.toggle("on");
      score.textContent = root.querySelectorAll("[data-d].on").length;
    });
  });
})();
</script>
