---
title: Robots as Tutors
permalink: /projects/robots-as-tutors/
layout: page
excerpt: Robot-assisted language learning research — does a bilingual robot tutor actually help, or just feel like it does?
comments: false
---
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@500;600;700&family=Nunito:wght@400;600;700;800&display=swap" rel="stylesheet">
<style>
/* Robots as Tutors page. Every rule is scoped to .rat and every class is prefixed rat-, so nothing here touches the rest of the site and the theme's own styles cannot leak in. Look: a kindergarten classroom wall, with alphabet blocks, crayon colors and cut-paper cards. Two rounded sans-serif fonts: Fredoka for headings, Nunito for text. */
.header:has(+ .page-content .rat){display:none}
.rat{--bg:#fdf7ec;--ink:#23304d;--muted:#5e6782;--card:#fff;--sh:#eadfc9;--line:rgba(35,48,77,.12);--sky:#3d9be9;--tomato:#f2643c;--sun:#ffc23d;--grass:#38b26b;--plum:#8a6ae0;--robin:#3d9be9;--deniz:#f2643c;--on:#1c2540;--rk:#23304d;
  --f-d:"Fredoka","Nunito",system-ui,-apple-system,"Segoe UI",sans-serif;--f-b:"Nunito",system-ui,-apple-system,"Segoe UI",Roboto,sans-serif;
  background:var(--bg);color:var(--ink);font-family:var(--f-b);font-size:18px;line-height:1.6;text-align:left;max-width:940px;margin:0 auto;padding:12px 30px 48px;border-radius:14px;overflow:hidden}
body[data-theme="dark"] .rat{--bg:#151b2e;--ink:#f4efe4;--muted:#a8b0c7;--card:#1f2740;--sh:#0b0f1d;--line:rgba(244,239,228,.12);--sky:#5fb0f2;--tomato:#ff7a52;--sun:#ffcd55;--grass:#4cc77f;--plum:#a58bf0;--robin:#5fb0f2;--deniz:#ff7a52}
.rat *,.rat *::before,.rat *::after{box-sizing:border-box}
.rat p{margin:0 0 14px;padding:0;opacity:1;max-width:690px;color:inherit}
.rat h1,.rat h2,.rat h3{font-family:var(--f-d);color:inherit;margin:0;padding:0;border:0;text-align:left;text-transform:none;letter-spacing:normal}
.rat h2::before,.rat h2::after,.rat h3::before,.rat h3::after{content:none}
.rat a{color:inherit}
.rat a::after{content:none!important}
.rat button{font-family:inherit}
.rat em,.rat i,.rat q,.rat cite{font-style:normal}
.rat b,.rat strong{color:inherit}
.rat ol,.rat ul{list-style:none!important;margin:0;padding:0}
.rat li{list-style:none!important}
.rat li::before{content:none}
.rat-k{font-family:var(--f-d);font-weight:600;font-size:14px;letter-spacing:.06em;text-transform:uppercase;color:var(--muted);margin-bottom:10px}

.rat-hero{position:relative;padding:40px 0 10px}
.rat p.rat-meta{font-weight:700;font-size:14px;color:var(--muted);margin:0 0 10px;max-width:none;padding-right:150px}
.rat h1.rat-title{font-weight:700;font-size:clamp(46px,9vw,92px);line-height:1.08;letter-spacing:-.02em;margin:0 0 22px;padding-right:150px}
.rat-blocks{display:inline-flex;gap:6px;vertical-align:baseline;flex-wrap:wrap}
.rat-blocks b{display:inline-grid;place-items:center;width:1.02em;height:1.06em;border-radius:.2em;color:#fff;font-weight:700;font-size:.92em;line-height:1;box-shadow:inset 0 -.1em 0 rgba(0,0,0,.18),0 .07em 0 rgba(0,0,0,.18);transition:transform .25s cubic-bezier(.34,1.56,.64,1)}
.rat-blocks b:nth-child(1){background:var(--tomato);transform:rotate(-5deg)}
.rat-blocks b:nth-child(2){background:var(--sun);color:#1c2540;transform:rotate(3deg) translateY(-.05em)}
.rat-blocks b:nth-child(3){background:var(--grass);transform:rotate(-2deg)}
.rat-blocks b:nth-child(4){background:var(--sky);transform:rotate(4deg) translateY(.04em)}
.rat-blocks b:nth-child(5){background:var(--plum);transform:rotate(-4deg)}
.rat-blocks b:nth-child(6){background:var(--tomato);transform:rotate(2deg) translateY(-.03em)}
.rat-blocks b:hover{transform:rotate(0) translateY(-.12em)}
.rat-herorow{margin-bottom:18px}
.rat-stamp{display:inline-block;background:var(--card);border-radius:999px;padding:8px 16px;font-weight:800;font-size:14px;box-shadow:0 5px 0 var(--sh)}
.rat-tags{display:flex;flex-wrap:wrap;gap:8px}
.rat-tags span{font-family:var(--f-d);font-weight:600;font-size:15px;padding:6px 14px;border-radius:999px;color:#1c2540}
.rat-tags span:nth-child(5n+1){background:#ffd9cc}.rat-tags span:nth-child(5n+2){background:#ffe9b0}.rat-tags span:nth-child(5n+3){background:#c9efd6}.rat-tags span:nth-child(5n+4){background:#cfe6fb}.rat-tags span:nth-child(5n){background:#e2d8fb}
.rat-herobots{position:absolute;right:0;top:40px;width:130px}
.rat-herobot{width:100%;height:auto;display:block}
.rat-herobot .head{transform-box:fill-box;transform-origin:50% 100%;animation:rat-wave 3.6s ease-in-out infinite}
@keyframes rat-wave{0%,100%{transform:rotate(0)}40%{transform:rotate(-6deg)}60%{transform:rotate(4deg)}}

.rat-short{margin:36px 0 0;background:var(--card);border-radius:28px;padding:24px 26px 18px;box-shadow:0 8px 0 var(--sh)}
.rat-short li{display:flex;gap:14px;align-items:flex-start;margin:0 0 14px!important;padding:0!important;font-family:var(--f-d);font-weight:500;font-size:clamp(18px,2.3vw,21px);line-height:1.35}
.rat-short li span{flex:0 0 38px;height:38px;border-radius:12px;display:grid;place-items:center;font-weight:700;font-size:19px;box-shadow:inset 0 -3px 0 rgba(0,0,0,.18)}
.rat .f1{--fc:var(--grass);--fo:#fff}.rat .f2{--fc:var(--plum);--fo:#fff}.rat .f3{--fc:var(--sun);--fo:#1c2540}
.rat-short li span{background:var(--fc);color:var(--fo)}

.rat-part{display:flex;align-items:center;gap:14px;flex-wrap:wrap;margin:64px 0 6px;font-family:var(--f-d);font-weight:700;font-size:clamp(30px,5vw,44px);line-height:1.1;letter-spacing:-.01em}
.rat-part span{font-size:14px;font-weight:600;letter-spacing:.08em;text-transform:uppercase;background:var(--ink);color:var(--bg);padding:6px 12px;border-radius:999px}
.rat-card{margin:24px 0 0;background:var(--card);border-radius:28px;padding:28px 30px 22px;box-shadow:0 8px 0 var(--sh)}
.rat h2.rat-h{display:flex;align-items:center;gap:14px;font-weight:700;font-size:clamp(26px,4vw,36px);line-height:1.1;margin:0 0 16px}
.rat-h span{flex:0 0 50px;height:50px;border-radius:15px;display:grid;place-items:center;background:var(--ink);color:var(--bg);font-size:18px;box-shadow:inset 0 -4px 0 rgba(0,0,0,.18)}
.rat-card p{font-size:18px}
.rat p.rat-ask{font-family:var(--f-d);font-weight:600;font-size:clamp(21px,3vw,26px);line-height:1.3;background:#fff3c8;color:#1c2540;border-radius:18px;padding:14px 18px;max-width:720px}
.rat p.rat-small{font-size:15px;color:var(--muted)}

.rat-lesson{margin:20px 0 6px;background:var(--bg);border-radius:24px;padding:18px}
.rat-pick{display:flex;flex-wrap:wrap;gap:8px;justify-content:center;margin-bottom:14px}
.rat-pick button{display:inline-flex;align-items:center;gap:8px;font-family:var(--f-d);font-weight:600;font-size:15px;border:2px solid var(--line);background:var(--card);color:var(--ink);border-radius:999px;padding:7px 14px;cursor:pointer}
.rat-pick button i{width:14px;height:14px;border-radius:50%;background:var(--robin)}
.rat-pick button[data-r="deniz"] i{background:var(--deniz)}
.rat-pick button.on{border-color:var(--ink);background:var(--ink);color:var(--bg)}
.rat-stage{display:grid;grid-template-columns:.85fr 1.5fr;gap:16px;align-items:end}
.rat-lesson[data-r="robin"]{--shirt:var(--robin)}
.rat-lesson[data-r="deniz"]{--shirt:var(--deniz)}
.rat-tutor{position:relative;display:flex;flex-direction:column;align-items:center;min-height:330px;justify-content:flex-end}
.rat-botwrap{width:min(190px,100%)}
.rat-bot{display:block;width:100%;height:auto}
.rat-name{font-family:var(--f-d);font-weight:700;font-size:16px;background:var(--shirt);color:#fff;border-radius:999px;padding:3px 14px;margin-top:6px;box-shadow:inset 0 -3px 0 rgba(0,0,0,.18)}
.rat-bub{position:absolute;left:0;right:0;top:0;margin:0 auto;width:max-content;max-width:100%;background:#fff;color:#1c2540;border:2.5px solid #1c2540;border-radius:18px;padding:9px 13px 10px;font-family:var(--f-d);font-weight:500;font-size:15.5px;line-height:1.3;box-shadow:4px 4px 0 #1c2540;z-index:3;opacity:0;visibility:hidden;transform:scale(.4) translateY(30px);transform-origin:50% 100%;transition:opacity .15s,transform .4s cubic-bezier(.34,1.56,.64,1),visibility 0s .4s}
.rat-bub::before,.rat-bub::after{content:"";position:absolute;clip-path:polygon(0 0,100% 0,50% 100%)}
.rat-bub::before{left:calc(50% - 12px);bottom:-17px;width:24px;height:17px;background:#1c2540}
.rat-bub::after{left:calc(50% - 8px);bottom:-11px;width:16px;height:12px;background:#fff}
.rat-lesson[data-say] .rat-bub{opacity:1;visibility:visible;transform:none;transition:opacity .15s,transform .4s cubic-bezier(.34,1.56,.64,1)}
.rat-bub b,.rat-tbub b,.rat-you b,.rat-legend span,.rat-who em{font-weight:700;border-radius:6px;padding:0 3px}
.rat .nl,.rat-bub b.nl,.rat-tbub b.nl,.rat-you b.nl{background:#cfe6fb;color:#123a66}
.rat .tr,.rat-bub b.tr{background:#ffd9cc;color:#7a2711}
.rat-desk{display:flex;flex-direction:column;gap:10px}
.rat-tablet{position:relative;background:#222838;border-radius:22px;padding:12px;box-shadow:0 6px 0 rgba(0,0,0,.18)}
.rat-scene{display:block;width:100%;height:auto;border-radius:12px;background:#cdeeff}
.rat-tbub{position:absolute;left:24px;top:22px;max-width:70%;background:#fff;color:#1c2540;border-radius:14px;padding:7px 12px;font-family:var(--f-d);font-weight:500;font-size:15px;box-shadow:0 4px 0 rgba(0,0,0,.18);z-index:2;opacity:0;transform:translateY(-6px);transition:.25s;pointer-events:none}
.rat-tbub::before{content:"🔊 ";font-size:13px}
.rat-lesson[data-step="2"] .rat-tbub{opacity:1;transform:none}
.rat-an{cursor:default;outline:none}
.rat-lesson[data-step="1"] .rat-an{cursor:pointer}
.rat-lesson[data-step="1"] .rat-an:hover,.rat-lesson[data-step="1"] .rat-an:focus-visible{filter:drop-shadow(0 0 6px #fff)}
.rat-an.rat-no{animation:rat-no .4s}
@keyframes rat-no{25%{transform:translateX(-4px)}75%{transform:translateX(4px)}}
.rat-scene .tree1{transform-box:fill-box;transform-origin:50% 100%;animation:rat-shake .5s ease-in-out infinite}
.rat-scene .monkey{transform-box:fill-box;transform-origin:0 50%;animation:rat-shake .5s ease-in-out infinite}
@keyframes rat-shake{0%,100%{transform:rotate(-2.5deg)}50%{transform:rotate(2.5deg)}}
.rat-scene .pawl{animation:rat-clapl .6s ease-in-out infinite}
.rat-scene .pawr{animation:rat-clapr .6s ease-in-out infinite}
@keyframes rat-clapl{0%,100%{transform:translateX(0)}50%{transform:translateX(11px)}}
@keyframes rat-clapr{0%,100%{transform:translateX(0)}50%{transform:translateX(-11px)}}
.rat-scene .bird{transform-box:fill-box;transform-origin:50% 100%;animation:rat-bob 1.6s ease-in-out infinite}
@keyframes rat-bob{0%,100%{transform:translateY(0)}50%{transform:translateY(-3px)}}
.rat-toys{display:flex;align-items:center;gap:12px;background:var(--card);border-radius:18px;padding:6px 14px;opacity:.45;transition:opacity .2s;outline:none}
.rat-toys span{font-family:var(--f-d);font-weight:600;font-size:14px;color:var(--muted)}
.rat-toyart{width:120px;height:auto;display:block}
.rat-toys.shake,.rat-toys.clap{opacity:1}
.rat-lesson[data-step="4"] .rat-toys{opacity:1;cursor:pointer;box-shadow:0 0 0 3px var(--sun)}
.rat-toyart .toy{transform-box:fill-box;transform-origin:50% 100%}
.rat-toys.shake .toy{animation:rat-shake .18s ease-in-out infinite}
.rat-toys.clap .toy{animation:rat-hopt .35s ease-in-out infinite}
.rat-toys.clap .t2{animation-delay:.17s}
@keyframes rat-hopt{0%,100%{transform:translateY(0)}50%{transform:translateY(-8px)}}
.rat-ctl{display:flex;flex-direction:column;align-items:center;gap:10px;margin-top:16px;text-align:center}
.rat-steps{display:flex;gap:8px;flex-wrap:wrap;justify-content:center}
.rat-steps span{font-family:var(--f-d);font-weight:600;font-size:13px;padding:4px 12px;border-radius:999px;background:var(--card);color:var(--muted);transition:.2s}
.rat-lesson[data-step="1"] .rat-steps span:nth-child(1),.rat-lesson[data-step="2"] .rat-steps span:nth-child(2),.rat-lesson[data-step="3"] .rat-steps span:nth-child(2),.rat-lesson[data-step="4"] .rat-steps span:nth-child(3){background:var(--sun);color:#1c2540}
.rat-you{font-family:var(--f-d);font-weight:600;font-size:17px;background:#e9f7ee;color:#1c4a2c;border-radius:16px;padding:6px 14px;display:none}
.rat-lesson[data-you] .rat-you{display:block}
.rat-hint{font-weight:700;font-size:15px;color:var(--muted);min-height:1.4em}
.rat-go{font-family:var(--f-d);font-weight:600;font-size:17px;border:0;background:var(--tomato);color:#fff;border-radius:16px;padding:11px 24px;cursor:pointer;box-shadow:inset 0 -4px 0 rgba(0,0,0,.2),0 4px 0 var(--sh)}
.rat-go:active{transform:translateY(2px)}
.rat-go[hidden]{display:none}
.rat-legend{display:flex;flex-wrap:wrap;gap:8px 12px;align-items:center;justify-content:center;margin-top:14px;font-size:13px;color:var(--muted)}
.rat-legend span{font-size:13px}


.rat h3.rat-st{font-weight:700;font-size:clamp(26px,4vw,36px);line-height:1.12;margin:0 0 14px}
.rat-pair{display:grid;grid-template-columns:1fr auto 1fr;gap:14px;align-items:stretch;margin:20px 0 18px}
.rat-who{background:var(--bg);border-radius:22px;padding:16px;text-align:center;display:flex;flex-direction:column;align-items:center;gap:2px}
.rat-mini{width:110px;height:auto;display:block;margin-bottom:6px}
.rat-who b{font-family:var(--f-d);font-weight:700;font-size:22px}
.rat-who span{font-weight:700;font-size:14px;color:var(--muted);margin-bottom:8px}
.rat-who q{font-family:var(--f-d);font-weight:500;font-size:15px;line-height:1.35;quotes:none}
.rat-who.robin b{color:var(--robin)}.rat-who.deniz b{color:var(--deniz)}
.rat-vs{align-self:center;font-family:var(--f-d);font-weight:600;font-size:15px;text-align:center;color:var(--muted);line-height:1.3}
.rat-flow{display:flex;flex-wrap:wrap;align-items:center;gap:8px;margin:6px 0 10px}
.rat-flow span{font-family:var(--f-d);font-weight:500;font-size:15px;background:var(--bg);border-radius:12px;padding:6px 12px}
.rat-flow span.later{background:#e2d8fb;color:#1c2540}
.rat-flow i{font-weight:700;color:var(--muted)}
.rat-plot{max-width:620px;margin:0 0 16px}
.rat-bars{width:100%;height:auto;display:block;overflow:visible}
.rat-bars .g{stroke:var(--line);stroke-width:1.5}
.rat-bars .ax{stroke:var(--ink);stroke-width:2.5}
.rat-bars .t{fill:var(--muted);font-family:var(--f-b);font-weight:700;font-size:14px}
.rat-bars .b{transform-box:fill-box;transform-origin:50% 100%;transform:scaleY(0);transition:transform .9s cubic-bezier(.34,1.3,.64,1)}
.rat-bars .b.robin{fill:var(--robin)}.rat-bars .b.deniz{fill:var(--deniz)}
.rat-bars .b.deniz{transition-delay:.12s}
.rat-in .rat-bars .b{transform:scaleY(1)}
.rat-bars .v{fill:var(--ink);font-family:var(--f-d);font-weight:700;font-size:22px}
.rat-bars .n{fill:var(--ink);font-family:var(--f-d);font-weight:600;font-size:16px}
.rat-bars .gl{fill:var(--muted);font-family:var(--f-d);font-weight:600;font-size:16px}
.rat-bars .ch{stroke:var(--ink);stroke-width:2;stroke-dasharray:7 6;opacity:.6}
.rat-bars .cht{fill:var(--muted);font-family:var(--f-b);font-weight:800;font-size:14px}
.rat-pref{display:flex;flex-wrap:wrap;align-items:center;gap:18px 26px;margin:0 0 16px}
.rat-dots{display:grid;grid-template-columns:repeat(17,1fr);gap:6px;width:min(100%,430px)}
.rat-dots i{aspect-ratio:1;border-radius:50%;background:var(--line);transform:scale(.3);transition:transform .35s cubic-bezier(.34,1.56,.64,1),background .2s;transition-delay:calc(var(--i)*14ms)}
.rat-in .rat-dots i{transform:scale(1)}
.rat-in .rat-dots i.d{background:var(--deniz)}
.rat-in .rat-dots i.r{background:var(--robin)}
.rat-prefkey{font-family:var(--f-d);font-weight:600;font-size:18px;display:flex;flex-direction:column;gap:6px}
.rat-prefkey b{font-size:34px;font-weight:700;margin-right:6px}
.rat-prefkey .d b{color:var(--deniz)}.rat-prefkey .r b{color:var(--robin)}
.rat-gap{display:grid;grid-template-columns:1fr 1fr;gap:12px;max-width:560px;margin-top:6px}
.rat-gap div{border-radius:20px;padding:14px 18px;color:#fff;--x:0;box-shadow:inset 0 -5px 0 rgba(0,0,0,.18)}
.rat-gap .d{background:var(--deniz)}.rat-gap .r{background:var(--robin)}
.rat-gap span{display:block;font-weight:800;font-size:14px;opacity:.9}
.rat-gap b{font-family:var(--f-d);font-weight:700;font-size:30px;line-height:1.1}

.rat-plan{margin:34px 0 0}
.rat-plangrid{display:grid;grid-template-columns:repeat(3,1fr);gap:12px}
.rat a.rat-plangrid a,.rat-plangrid a{display:block;text-decoration:none;background:var(--card);color:var(--ink);border-radius:20px;padding:14px 16px 16px;font-family:var(--f-d);font-weight:600;font-size:18px;line-height:1.25;box-shadow:0 6px 0 var(--sh);border-top:7px solid var(--fc);transition:transform .15s}
.rat .rat-plangrid a,.rat .rat-plangrid a:visited{color:var(--ink)!important}
.rat-plangrid a:hover{transform:translateY(-2px)}
.rat-plangrid a span{display:block;font-size:12px;letter-spacing:.08em;text-transform:uppercase;color:var(--muted);margin-bottom:4px}
.rat-ch{position:relative;display:grid;grid-template-columns:64px 1fr;gap:18px;margin:28px 0 0;scroll-margin-top:20px}
.rat-ch::before{content:"";position:absolute;left:30px;top:70px;bottom:-30px;border-left:3px dashed var(--line)}
.rat-chn{position:relative;width:64px;height:64px;border-radius:20px;display:grid;place-items:center;background:var(--fc);color:var(--fo);font-family:var(--f-d);font-weight:700;font-size:30px;box-shadow:inset 0 -5px 0 rgba(0,0,0,.18)}
.rat-chb{background:var(--card);border-radius:28px;padding:24px 26px 18px;box-shadow:0 8px 0 var(--sh);min-width:0}
.rat-chk{font-family:var(--f-d);font-weight:600;font-size:13px;letter-spacing:.08em;text-transform:uppercase;color:var(--muted);margin-bottom:6px}
.rat h3.rat-cht{font-weight:600;font-size:clamp(23px,3.4vw,30px);line-height:1.2;margin:0 0 16px}
.rat-guess{background:var(--bg);border-radius:22px;padding:16px 18px 6px;margin:0 0 16px}
.rat p.rat-gq{font-family:var(--f-d);font-weight:600;font-size:18px;margin:0 0 10px}
.rat-gb{display:flex;flex-wrap:wrap;gap:10px;margin-bottom:12px}
.rat-gb button{display:inline-flex;align-items:center;gap:8px;font-family:var(--f-d);font-weight:600;font-size:17px;border:0;background:var(--card);color:var(--ink);border-radius:16px;padding:10px 18px;cursor:pointer;box-shadow:0 4px 0 var(--sh);transition:transform .15s}
.rat-gb button:hover{transform:translateY(-2px)}
.rat-gb button i{width:14px;height:14px;border-radius:50%;background:var(--robin)}
.rat-gb button[data-g="deniz"] i{background:var(--deniz)}
.rat-ch[data-g] .rat-gb button{cursor:default;opacity:.45;transform:none}
.rat-ch[data-g="robin"] .rat-gb button[data-g="robin"],.rat-ch[data-g="deniz"] .rat-gb button[data-g="deniz"]{opacity:1;box-shadow:0 0 0 3px var(--ink)}
.rat-guess .rat-plot{transition:filter .5s,opacity .5s}
.rat-guess .rat-pref{transition:filter .5s,opacity .5s}
.rat-ch[data-guess]:not([data-g]) .rat-guess .rat-plot,.rat-ch[data-guess]:not([data-g]) .rat-guess .rat-pref{filter:blur(7px);opacity:.45}
.rat p.rat-gmsg{font-family:var(--f-d);font-weight:600;font-size:18px;min-height:0;margin:0 0 10px}
.rat-ch[data-guess]:not([data-g]) .rat-after{display:none}
.rat-after{animation:rat-up .5s ease-out}
@keyframes rat-up{from{opacity:0;transform:translateY(10px)}to{opacity:1;transform:none}}
.rat-verdict{display:inline-flex;align-items:center;gap:10px;font-family:var(--f-d);font-weight:600;font-size:18px;background:var(--bg);border-radius:999px;padding:6px 16px 6px 6px;margin:4px 0 16px}
.rat-verdict b{width:32px;height:32px;border-radius:50%;display:grid;place-items:center;color:#fff;font-size:17px}
.rat-verdict.yes b{background:var(--grass)}
.rat-verdict.no b{background:#e5484d}
.rat-find{font-family:var(--f-d);font-weight:600;font-size:clamp(19px,2.6vw,23px);line-height:1.28;margin:0 0 14px;max-width:760px}
.rat-find span{display:inline-block;font-size:13px;letter-spacing:.08em;text-transform:uppercase;background:var(--fc);color:var(--fo);border-radius:999px;padding:3px 11px;margin:0 10px 6px 0;vertical-align:middle}
.rat-test{background:var(--bg);border-radius:22px;padding:18px;margin:6px 0 16px;text-align:center}
.rat-tq{display:flex;flex-wrap:wrap;align-items:center;justify-content:center;gap:4px 10px;font-family:var(--f-d);font-weight:600;font-size:22px;margin-bottom:14px}
.rat-tq small{flex-basis:100%;font-size:15px;color:var(--muted)}
.rat-tcards{display:grid;grid-template-columns:repeat(3,1fr);gap:12px;max-width:520px;margin:0 auto}
.rat-tcards button{border:0;padding:6px;background:#222838;border-radius:16px;cursor:pointer;box-shadow:0 5px 0 var(--sh);transition:transform .15s,box-shadow .2s}
.rat-tcards button:hover{transform:translateY(-3px)}
.rat-tcards svg{display:block;width:100%;height:auto;border-radius:11px}
.rat-tcards button.ok{box-shadow:0 0 0 4px var(--grass),0 5px 0 var(--sh)}
.rat-tcards button.no{animation:rat-no .4s;box-shadow:0 0 0 4px #e5484d,0 5px 0 var(--sh)}
.rat-tcards .tree1,.rat-tcards .monkey{transform-box:fill-box;transform-origin:50% 100%;animation:rat-shake .5s ease-in-out infinite}
.rat-tcards .pawl{animation:rat-clapl2 .6s ease-in-out infinite}
.rat-tcards .pawr{animation:rat-clapr2 .6s ease-in-out infinite}
@keyframes rat-clapl2{0%,100%{transform:translateX(0)}50%{transform:translateX(8px)}}
@keyframes rat-clapr2{0%,100%{transform:translateX(0)}50%{transform:translateX(-8px)}}
.rat-tcards .wing{transform-box:fill-box;transform-origin:0 100%;animation:rat-flap .35s ease-in-out infinite alternate}
@keyframes rat-flap{from{transform:rotate(0)}to{transform:rotate(-35deg)}}
.rat-tcards .bird{animation:rat-bob 1.2s ease-in-out infinite}
.rat p.rat-tmsg{font-family:var(--f-d);font-weight:600;font-size:17px;margin:14px auto 0;max-width:none}
.rat-whyx{margin:44px 0 0;background:#5b45b0;color:#fff;border-radius:30px;padding:30px 30px 22px;box-shadow:inset 0 -8px 0 rgba(0,0,0,.18)}
body[data-theme="dark"] .rat-whyx{background:#4a3a96}
.rat h3.rat-whyh{font-weight:700;font-size:clamp(26px,4vw,36px);line-height:1.15;margin:0 0 20px;color:#fff}
.rat-reasons{display:grid;grid-template-columns:repeat(3,1fr);gap:14px}
.rat-reasons div{background:#fff;color:#1c2540;border-radius:22px;padding:18px 18px 8px;box-shadow:0 6px 0 rgba(0,0,0,.18)}
.rat-reasons b{display:grid;place-items:center;width:40px;height:40px;border-radius:13px;background:var(--sun);color:#1c2540;font-family:var(--f-d);font-weight:700;font-size:20px;margin-bottom:10px;box-shadow:inset 0 -3px 0 rgba(0,0,0,.15)}
.rat .rat-reasons strong{display:block;font-family:var(--f-d);font-weight:700;font-size:21px;margin-bottom:6px;color:#1c2540}
.rat-reasons p{font-size:16px;line-height:1.5}
.rat p.rat-whynote{margin:16px 0 0;font-size:14px;font-weight:700;opacity:.85}
.rat-biz{display:grid;grid-template-columns:repeat(3,1fr);gap:16px;margin-top:24px}
.rat-bcard{background:var(--card);border-radius:24px;padding:20px 20px 8px;box-shadow:0 8px 0 var(--sh);display:flex;flex-direction:column}
.rat-bcard span{align-self:flex-start;font-family:var(--f-d);font-weight:600;font-size:13px;letter-spacing:.08em;text-transform:uppercase;background:var(--fc);color:var(--fo);border-radius:999px;padding:3px 11px;margin-bottom:12px}
.rat-bcard b{font-family:var(--f-d);font-weight:600;font-size:19px;line-height:1.25;margin-bottom:12px}
.rat-bcard p{font-size:15.5px;line-height:1.5;color:var(--muted)}
.rat-take{margin:40px 0 0;background:var(--sky);color:#fff;border-radius:28px;padding:28px 30px;box-shadow:inset 0 -8px 0 rgba(0,0,0,.15)}
.rat-take .rat-k{color:#fff;opacity:.85}
.rat-take p{font-family:var(--f-d);font-weight:600;font-size:clamp(21px,3vw,27px);line-height:1.3;margin:0;max-width:780px}
.rat-actions{display:flex;flex-wrap:wrap;gap:12px;margin:34px 0 4px}
.rat a.rat-btn{display:inline-block;text-decoration:none;font-family:var(--f-d);font-weight:600;font-size:17px;padding:12px 22px;border-radius:16px;background:var(--sun);color:#1c2540;box-shadow:inset 0 -4px 0 rgba(0,0,0,.15),0 4px 0 var(--sh);transition:transform .15s}
.rat a.rat-btn.alt{background:var(--card);color:var(--ink)}
.rat a.rat-btn:hover{transform:translateY(-2px)}

.rat-bot .head,.rat-bot .body,.rat-bot .eye,.rat-bot .mouth,.rat-mini .eye{transform-box:fill-box;transform-origin:50% 100%}
.rat-bot .head{animation:rat-sway 6s ease-in-out infinite}
.rat-bot .body{animation:rat-breath 4s ease-in-out infinite}
.rat-bot .eye,.rat-mini .eye,.rat-herobot .eye{transform-box:fill-box;transform-origin:50% 50%;animation:rat-blink 4.8s infinite}
.rat-bot .pupil{transition:transform .12s}
.rat-lesson[data-talk] .rat-bot .mouth{animation:rat-talk .2s infinite alternate;transform-origin:50% 50%}
.rat-lesson[data-happy] .rat-bot .head{animation:rat-hop .55s ease-out}
.rat-bot.nod .head{animation:rat-nod .4s ease-out}
@keyframes rat-sway{0%,100%{transform:translateY(0) rotate(0)}30%{transform:translateY(-2px) rotate(1.6deg)}65%{transform:translateY(1px) rotate(-1.4deg)}}
@keyframes rat-breath{0%,100%{transform:scaleY(1)}50%{transform:scaleY(1.025)}}
@keyframes rat-blink{0%,93%,100%{transform:scaleY(1)}96%{transform:scaleY(.08)}}
@keyframes rat-talk{from{transform:scaleY(.4)}to{transform:scaleY(1.5)}}
@keyframes rat-hop{0%{transform:translateY(0)}35%{transform:translateY(-8px)}100%{transform:translateY(0)}}
@keyframes rat-nod{0%,100%{transform:translateY(0)}40%{transform:translateY(5px)}}

@media(max-width:760px){.rat-biz,.rat-plangrid,.rat-reasons{grid-template-columns:1fr}.rat-whyx{padding:24px 16px 18px}.rat-ch{grid-template-columns:44px 1fr;gap:10px}.rat-chn{width:44px;height:44px;font-size:22px;border-radius:14px}.rat-ch::before{left:20px;top:50px}.rat-chb{padding:18px 12px 12px}.rat-guess{padding:12px 8px 4px}.rat-ch{grid-template-columns:36px 1fr;gap:8px}.rat-chn{width:36px;height:36px;font-size:19px;border-radius:12px}.rat-ch::before{left:16px;top:44px}.rat-stage{grid-template-columns:1fr}.rat-tutor{min-height:290px}.rat-pair{grid-template-columns:1fr}.rat-vs br{display:none}}
@media(max-width:600px){.rat{padding:8px 16px 34px;font-size:16px}.rat-herobots{display:none}.rat p.rat-meta,.rat h1.rat-title{padding-right:0}.rat-card{padding:22px 18px 16px}.rat-lesson{padding:12px;margin-inline:-6px}.rat-h span{flex-basis:42px;height:42px;font-size:15px}.rat-dots{gap:4px}.rat-gap b{font-size:24px}.rat-bars .v{font-size:30px}.rat-bars .n{font-size:21px}.rat-bars .gl{font-size:19px}.rat-bars .t{font-size:18px}.rat-bars .cht{font-size:17px}.rat-bub{font-size:14px}}
@media(prefers-reduced-motion:reduce){.rat *{animation:none!important;transition:none!important}.rat-bars .b,.rat-dots i{transform:none!important}}
</style>
<div class="rat">
<div class="rat-hero">
  <p class="rat-meta">Robot-assisted language learning research · Tilburg &amp; Utrecht Universities · 2017–2018</p>
  <h1 class="rat-title">Robots as <span class="rat-blocks" aria-label="Tutors"><b>T</b><b>U</b><b>T</b><b>O</b><b>R</b><b>S</b></span></h1>
  <div class="rat-herorow">
    <span class="rat-stamp">Published in the Journal of Computer Assisted Learning, 2021</span>
  </div>
  <div class="rat-tags" aria-label="Skills"><span>A/B Testing</span><span>Bilingual Education</span><span>Mixed-Effects Models</span><span>R</span><span>Multi-Site Collaboration</span></div>
  <div class="rat-herobots" aria-hidden="true"><svg class="rat-herobot" viewBox="0 0 160 150" aria-hidden="true">
<g class="body"><path d="M24 150C24 118 50 106 80 106C110 106 136 118 136 150Z" fill="var(--robin)" stroke="var(--rk)" stroke-width="4"/><path d="M62 108L80 126L98 108" fill="none" stroke="var(--rk)" stroke-width="3.5" stroke-linejoin="round"/></g>
<g class="head">
<line x1="80" y1="10" x2="80" y2="24" stroke="var(--rk)" stroke-width="4" stroke-linecap="round"/>
<circle class="ant" cx="80" cy="8" r="5.5" fill="var(--sun)"/>
<rect x="34" y="22" width="92" height="72" rx="26" fill="#fff" stroke="var(--rk)" stroke-width="4"/>
<g class="eye"><circle cx="60" cy="54" r="12" fill="#fff" stroke="var(--rk)" stroke-width="3"/><circle class="pupil" cx="60" cy="54" r="5.5" fill="var(--rk)"/></g>
<g class="eye"><circle cx="100" cy="54" r="12" fill="#fff" stroke="var(--rk)" stroke-width="3"/><circle class="pupil" cx="100" cy="54" r="5.5" fill="var(--rk)"/></g>
<ellipse class="mouth" cx="80" cy="78" rx="6" ry="4.5" fill="var(--tomato)"/>
</g></svg></div>
</div>
<div class="rat-short">
  <div class="rat-k">The short version</div>
  <ol>
    <li class="f1"><span>1</span>Children learned more Dutch words from the Dutch-only robot than from the robot that added Turkish translations.</li>
    <li class="f2"><span>2</span>Most children preferred the bilingual robot, but their preference did not change how much they learned.</li>
    <li class="f3"><span>3</span>Children who already knew more words, in Turkish or in Dutch, learned more from both robots.</li>
  </ol>
</div>
<div class="rat-part"><span>Part one</span>The setup</div>
<div class="rat-card">
  <h2 class="rat-h"><span>01</span>The question</h2>
  <p>Classrooms are increasingly mixed in terms of what languages children speak at home, and teachers cannot realistically give every child support in their own first language. A robot, however, can be programmed to speak more than one language.</p>
  <p class="rat-ask">When a robot teaches a child a new word in a second language, should it also give the translation in the child's first language?</p>
  <p>The study focused on Turkish-Dutch kindergartners, a group whose Dutch language skills and school outcomes tend to lag behind their monolingual Dutch peers. The aim was not to replace teachers, but to test whether a robot could offer one-on-one language support alongside them. The project was part of <a href="http://l2tor.eu" target="_blank" rel="noopener">L2TOR</a>, funded by the European Union's Horizon 2020 programme.</p>
</div>
<div class="rat-card">
  <h2 class="rat-h"><span>02</span>The lesson</h2>
  <p>67 Turkish-Dutch kindergartners, aged 4 to 6, each learned six Dutch words from a robot through a tablet game. Each child already knew these words in Turkish, but not yet in Dutch. Play a round below: you are the child.</p>
  <div class="rat-lesson" id="rat-lesson" data-r="robin" data-step="0">
    <div class="rat-pick" role="group" aria-label="Which robot teaches">
      <button type="button" data-r="robin" class="on" aria-pressed="true"><i></i>Robin · Dutch only</button>
      <button type="button" data-r="deniz" aria-pressed="false"><i></i>Deniz · Dutch + Turkish</button>
    </div>
    <div class="rat-stage">
      <div class="rat-tutor">
        <div class="rat-bub" id="rat-bub" aria-live="polite"></div>
        <div class="rat-botwrap" id="rat-bot"><svg class="rat-bot" viewBox="0 0 160 150" aria-hidden="true">
<g class="body"><path d="M24 150C24 118 50 106 80 106C110 106 136 118 136 150Z" fill="var(--shirt)" stroke="var(--rk)" stroke-width="4"/><path d="M62 108L80 126L98 108" fill="none" stroke="var(--rk)" stroke-width="3.5" stroke-linejoin="round"/></g>
<g class="head">
<line x1="80" y1="10" x2="80" y2="24" stroke="var(--rk)" stroke-width="4" stroke-linecap="round"/>
<circle class="ant" cx="80" cy="8" r="5.5" fill="var(--sun)"/>
<rect x="34" y="22" width="92" height="72" rx="26" fill="#fff" stroke="var(--rk)" stroke-width="4"/>
<g class="eye"><circle cx="60" cy="54" r="12" fill="#fff" stroke="var(--rk)" stroke-width="3"/><circle class="pupil" cx="60" cy="54" r="5.5" fill="var(--rk)"/></g>
<g class="eye"><circle cx="100" cy="54" r="12" fill="#fff" stroke="var(--rk)" stroke-width="3"/><circle class="pupil" cx="100" cy="54" r="5.5" fill="var(--rk)"/></g>
<ellipse class="mouth" cx="80" cy="78" rx="6" ry="4.5" fill="var(--tomato)"/>
</g></svg></div>
        <div class="rat-name" id="rat-name">Robin</div>
      </div>
      <div class="rat-desk">
        <div class="rat-tablet">
          <div class="rat-tbub" id="rat-tbub"></div>
          <svg class="rat-scene" viewBox="0 0 400 230" aria-label="Forest picture on the tablet">
<rect width="400" height="230" fill="#cdeeff"/>
<circle cx="360" cy="34" r="20" fill="#ffd95e"/>
<path d="M0 168C80 156 150 176 220 166C290 156 340 170 400 162V230H0Z" fill="#9edb8c"/>
<g class="rat-an" data-an="monkey" role="button" tabindex="0" aria-label="Monkey">
 <g class="tree1"><rect x="98" y="92" width="22" height="88" rx="6" fill="#8b5a3c"/><circle cx="109" cy="74" r="40" fill="#3fae6a"/><circle cx="76" cy="96" r="26" fill="#36a160"/><circle cx="142" cy="96" r="26" fill="#36a160"/></g>
 <g class="monkey"><path d="M150 168C146 176 152 182 158 178" fill="none" stroke="#7a5233" stroke-width="5" stroke-linecap="round"/><ellipse cx="146" cy="152" rx="14" ry="18" fill="#9b6b43"/><path d="M136 144L120 132" stroke="#9b6b43" stroke-width="7" stroke-linecap="round"/><path d="M137 156L120 150" stroke="#9b6b43" stroke-width="7" stroke-linecap="round"/><circle cx="148" cy="128" r="13" fill="#9b6b43"/><circle cx="136" cy="124" r="5" fill="#9b6b43"/><circle cx="160" cy="124" r="5" fill="#9b6b43"/><ellipse cx="149" cy="131" rx="8" ry="7" fill="#f2cfa4"/><circle cx="145" cy="128" r="1.8" fill="#222"/><circle cx="152" cy="128" r="1.8" fill="#222"/></g>
</g>
<g class="rat-an" data-an="bear" role="button" tabindex="0" aria-label="Bear">
 <g class="bear"><ellipse cx="258" cy="160" rx="26" ry="30" fill="#7a5136"/><ellipse cx="258" cy="166" rx="15" ry="18" fill="#a77a55"/><circle cx="242" cy="108" r="8" fill="#7a5136"/><circle cx="274" cy="108" r="8" fill="#7a5136"/><circle cx="258" cy="120" r="19" fill="#7a5136"/><ellipse cx="258" cy="126" rx="8" ry="6" fill="#a77a55"/><circle cx="258" cy="124" r="2.4" fill="#222"/><circle cx="251" cy="116" r="2" fill="#222"/><circle cx="265" cy="116" r="2" fill="#222"/>
 <g class="pawl"><circle cx="240" cy="150" r="7" fill="#6a452d"/></g><g class="pawr"><circle cx="276" cy="150" r="7" fill="#6a452d"/></g></g>
</g>
<g><rect x="334" y="104" width="16" height="76" rx="5" fill="#8b5a3c"/><circle cx="342" cy="96" r="30" fill="#3fae6a"/></g>
<g class="rat-an" data-an="bird" role="button" tabindex="0" aria-label="Bird">
 <g class="bird"><ellipse cx="318" cy="76" rx="10" ry="8" fill="#ff8a5b"/><circle cx="310" cy="70" r="6" fill="#ff8a5b"/><path d="M304 70L298 72L304 74Z" fill="#f2b51d"/><circle cx="309" cy="69" r="1.4" fill="#222"/></g>
</g>
</svg>
        </div>
        <div class="rat-toys" id="rat-toys" role="button" tabindex="0" aria-label="Toys"><svg class="rat-toyart" viewBox="0 0 170 70" aria-hidden="true">
<g class="toy t1"><circle cx="48" cy="40" r="20" fill="#c99566"/><circle cx="33" cy="22" r="7" fill="#c99566"/><circle cx="63" cy="22" r="7" fill="#c99566"/><circle cx="48" cy="44" r="7" fill="#e8c6a0"/><circle cx="42" cy="36" r="2.2" fill="#222"/><circle cx="54" cy="36" r="2.2" fill="#222"/></g>
<g class="toy t2"><ellipse cx="120" cy="44" rx="19" ry="18" fill="#f6d7e3"/><ellipse cx="112" cy="16" rx="5" ry="13" fill="#f6d7e3"/><ellipse cx="128" cy="16" rx="5" ry="13" fill="#f6d7e3"/><circle cx="114" cy="40" r="2.2" fill="#222"/><circle cx="126" cy="40" r="2.2" fill="#222"/><circle cx="120" cy="47" r="2.5" fill="#e98aa8"/></g>
</svg><span>Your toys</span></div>
      </div>
    </div>
    <div class="rat-ctl">
      <div class="rat-steps" aria-hidden="true"><span>1 · Find it</span><span>2 · Say it</span><span>3 · Act it out</span></div>
      <div class="rat-you" id="rat-you"></div>
      <div class="rat-hint" id="rat-hint">Pick a robot, then start.</div>
      <button type="button" class="rat-go" id="rat-go">Start the lesson</button>
    </div>
    <div class="rat-legend"><span class="nl">Dutch word</span><span class="tr">Turkish word</span><em>The robot spoke Dutch. Its lines are shown in English.</em></div>
  </div>
</div>
<div class="rat-card">
  <h2 class="rat-h"><span>03</span>The test</h2>
  <p>To check which words stuck, children heard a Dutch word and picked the matching picture out of three. Try one:</p>
  <div class="rat-test" id="rat-test">
    <div class="rat-tq"><span aria-hidden="true">🔊</span><span>“<b class="nl">Klappen</b>”</span><small>Which picture shows it?</small></div>
    <div class="rat-tcards">
      <button type="button" data-ok="0" aria-label="Monkey shaking a tree"><svg viewBox="0 0 120 96" aria-hidden="true"><rect width="120" height="96" fill="#cdeeff"/><rect y="74" width="120" height="22" fill="#9edb8c"/><g class="tree1"><rect x="44" y="40" width="12" height="40" rx="4" fill="#8b5a3c"/><circle cx="50" cy="32" r="22" fill="#3fae6a"/></g><g class="monkey"><ellipse cx="68" cy="66" rx="8" ry="10" fill="#9b6b43"/><path d="M62 60L54 54" stroke="#9b6b43" stroke-width="5" stroke-linecap="round"/><circle cx="69" cy="52" r="7" fill="#9b6b43"/><ellipse cx="69.5" cy="54" rx="4.5" ry="4" fill="#f2cfa4"/></g></svg></button>
      <button type="button" data-ok="1" aria-label="Bear clapping"><svg viewBox="0 0 120 96" aria-hidden="true"><rect width="120" height="96" fill="#cdeeff"/><rect y="74" width="120" height="22" fill="#9edb8c"/><g class="bear"><ellipse cx="60" cy="66" rx="17" ry="20" fill="#7a5136"/><ellipse cx="60" cy="70" rx="10" ry="12" fill="#a77a55"/><circle cx="49" cy="32" r="5.5" fill="#7a5136"/><circle cx="71" cy="32" r="5.5" fill="#7a5136"/><circle cx="60" cy="40" r="13" fill="#7a5136"/><ellipse cx="60" cy="44" rx="5.5" ry="4" fill="#a77a55"/><circle cx="55" cy="38" r="1.5" fill="#222"/><circle cx="65" cy="38" r="1.5" fill="#222"/><g class="pawl"><circle cx="47" cy="60" r="5" fill="#6a452d"/></g><g class="pawr"><circle cx="73" cy="60" r="5" fill="#6a452d"/></g></g></svg></button>
      <button type="button" data-ok="0" aria-label="Bird flying"><svg viewBox="0 0 120 96" aria-hidden="true"><rect width="120" height="96" fill="#cdeeff"/><rect y="74" width="120" height="22" fill="#9edb8c"/><g class="bird"><ellipse cx="60" cy="46" rx="13" ry="10" fill="#ff8a5b"/><circle cx="50" cy="40" r="7" fill="#ff8a5b"/><path d="M43 40L36 42L43 44Z" fill="#f2b51d"/><circle cx="49" cy="39" r="1.6" fill="#222"/><path class="wing" d="M60 42Q70 26 80 34Q72 44 60 46Z" fill="#e5703f"/></g></svg></button>
    </div>
    <p class="rat-tmsg" id="rat-tmsg">Tap a picture.</p>
  </div>
  <p>Each word was tested three times, right after the lesson and again about a week later. Guessing alone gets one in three right (33%), so scores above that mean children really learned the words.</p>
</div>
<div class="rat-part"><span>Part two</span>The experiment</div>
<div class="rat-card rat-exp">
  <h3 class="rat-st">Do Turkish translations help children learn Dutch words?</h3>
  <p>Every child met two robots. Robin spoke only Dutch. Deniz spoke Dutch and also gave the Turkish translation of each new word. Each robot taught three of the child's six words.</p>
  <div class="rat-pair">
    <div class="rat-who robin"><svg class="rat-mini" viewBox="0 0 160 150" aria-hidden="true">
<g class="body"><path d="M24 150C24 118 50 106 80 106C110 106 136 118 136 150Z" fill="var(--robin)" stroke="var(--rk)" stroke-width="4"/><path d="M62 108L80 126L98 108" fill="none" stroke="var(--rk)" stroke-width="3.5" stroke-linejoin="round"/></g>
<g class="head">
<line x1="80" y1="10" x2="80" y2="24" stroke="var(--rk)" stroke-width="4" stroke-linecap="round"/>
<circle class="ant" cx="80" cy="8" r="5.5" fill="var(--sun)"/>
<rect x="34" y="22" width="92" height="72" rx="26" fill="#fff" stroke="var(--rk)" stroke-width="4"/>
<g class="eye"><circle cx="60" cy="54" r="12" fill="#fff" stroke="var(--rk)" stroke-width="3"/><circle class="pupil" cx="60" cy="54" r="5.5" fill="var(--rk)"/></g>
<g class="eye"><circle cx="100" cy="54" r="12" fill="#fff" stroke="var(--rk)" stroke-width="3"/><circle class="pupil" cx="100" cy="54" r="5.5" fill="var(--rk)"/></g>
<ellipse class="mouth" cx="80" cy="78" rx="6" ry="4.5" fill="var(--tomato)"/>
</g></svg><b>Robin</b><span>Dutch only</span><q>“In Dutch we say <em class="nl">schudden</em>.”</q></div>
    <div class="rat-vs">Same robot. <br>Different shirt.</div>
    <div class="rat-who deniz"><svg class="rat-mini" viewBox="0 0 160 150" aria-hidden="true">
<g class="body"><path d="M24 150C24 118 50 106 80 106C110 106 136 118 136 150Z" fill="var(--deniz)" stroke="var(--rk)" stroke-width="4"/><path d="M62 108L80 126L98 108" fill="none" stroke="var(--rk)" stroke-width="3.5" stroke-linejoin="round"/></g>
<g class="head">
<line x1="80" y1="10" x2="80" y2="24" stroke="var(--rk)" stroke-width="4" stroke-linecap="round"/>
<circle class="ant" cx="80" cy="8" r="5.5" fill="var(--sun)"/>
<rect x="34" y="22" width="92" height="72" rx="26" fill="#fff" stroke="var(--rk)" stroke-width="4"/>
<g class="eye"><circle cx="60" cy="54" r="12" fill="#fff" stroke="var(--rk)" stroke-width="3"/><circle class="pupil" cx="60" cy="54" r="5.5" fill="var(--rk)"/></g>
<g class="eye"><circle cx="100" cy="54" r="12" fill="#fff" stroke="var(--rk)" stroke-width="3"/><circle class="pupil" cx="100" cy="54" r="5.5" fill="var(--rk)"/></g>
<ellipse class="mouth" cx="80" cy="78" rx="6" ry="4.5" fill="var(--tomato)"/>
</g></svg><b>Deniz</b><span>Dutch + Turkish</span><q>“So it is <em class="tr">sallamak</em> in Turkish and <em class="nl">schudden</em> in Dutch.”</q></div>
  </div>
  <div class="rat-flow" aria-label="Session order">
    <span>Lesson with one robot</span><i>→</i><span>Shirt change</span><i>→</i><span>Lesson with the other robot</span><i>→</i><span>“Which robot do you want to play with again?”</span><i>→</i><span>Test</span><i>→</i><span class="later">A week later: test again</span>
  </div>
  <p class="rat-small">Half of the children met Robin first and half met Deniz first, so the order could not favor either robot.</p>
</div>
<div class="rat-plan">
  <div class="rat-k">Going in, the team had two predictions and one open question</div>
  <div class="rat-plangrid">
    <a href="#rat-ch1" class="f1"><span>Prediction 1</span>Translations help children learn</a>
    <a href="#rat-ch2" class="f2"><span>Prediction 2</span>Children prefer the bilingual robot</a>
    <a href="#rat-ch3" class="f3"><span>Open question</span>Does what children already know matter?</a>
  </div>
</div>
<div class="rat-ch f1" id="rat-ch1" data-guess>
  <div class="rat-chn">1</div>
  <div class="rat-chb">
    <div class="rat-chk">Prediction 1</div>
    <h3 class="rat-cht">Turkish translations will help children learn Dutch words.</h3>
    <div class="rat-guess">
      <p class="rat-gq">Your guess: whose words did children remember better?</p>
      <div class="rat-gb"><button type="button" data-g="robin" data-msg="Good call. The team expected the opposite."><i></i>Robin's</button><button type="button" data-g="deniz" data-msg="That was the team's prediction too."><i></i>Deniz's</button></div>
      <div class="rat-plot"><svg class="rat-bars" viewBox="0 0 640 320" role="img" aria-label="Correct answers by robot. Right after the lesson: Robin 66%, Deniz 62%. A week later: Robin 69%, Deniz 69%. Chance is 33%."><line class="g" x1="64" x2="624" y1="246.0" y2="246.0"/><text class="t" x="54" y="251.0" text-anchor="end">0%</text><line class="g" x1="64" x2="624" y1="189.0" y2="189.0"/><text class="t" x="54" y="194.0" text-anchor="end">25%</text><line class="g" x1="64" x2="624" y1="132.0" y2="132.0"/><text class="t" x="54" y="137.0" text-anchor="end">50%</text><line class="g" x1="64" x2="624" y1="75.0" y2="75.0"/><text class="t" x="54" y="80.0" text-anchor="end">75%</text><line class="g" x1="64" x2="624" y1="18.0" y2="18.0"/><text class="t" x="54" y="23.0" text-anchor="end">100%</text><line class="ch" x1="64" x2="624" y1="170.0" y2="170.0"/><text class="cht" x="344.0" y="142.0" text-anchor="middle">Chance</text><text class="cht" x="344.0" y="160.0" text-anchor="middle">33%</text><rect class="b robin" x="130.2" y="95.5" width="78" height="150.5" rx="10"><title>Right after the lesson, Robin: 66%</title></rect><text class="v" x="169.2" y="85.5" text-anchor="middle">66%</text><text class="n" x="169.2" y="268.0" text-anchor="middle">Robin</text><rect class="b deniz" x="222.2" y="104.6" width="78" height="141.4" rx="10"><title>Right after the lesson, Deniz: 62%</title></rect><text class="v" x="261.2" y="94.6" text-anchor="middle">62%</text><text class="n" x="261.2" y="268.0" text-anchor="middle">Deniz</text><text class="gl" x="215.2" y="298.0" text-anchor="middle">Right after the lesson</text><rect class="b robin" x="387.8" y="88.7" width="78" height="157.3" rx="10"><title>A week later, Robin: 69%</title></rect><text class="v" x="426.8" y="78.7" text-anchor="middle">69%</text><text class="n" x="426.8" y="268.0" text-anchor="middle">Robin</text><rect class="b deniz" x="479.8" y="88.7" width="78" height="157.3" rx="10"><title>A week later, Deniz: 69%</title></rect><text class="v" x="518.8" y="78.7" text-anchor="middle">69%</text><text class="n" x="518.8" y="268.0" text-anchor="middle">Deniz</text><text class="gl" x="472.8" y="298.0" text-anchor="middle">A week later</text><line class="ax" x1="64" x2="624" y1="246" y2="246"/></svg></div>
      <p class="rat-gmsg"></p>
    </div>
    <div class="rat-after">
      <div class="rat-verdict no"><b>✗</b>Not supported. The opposite happened.</div>
      <div class="rat-find"><span>Finding 1</span>Children learned more Dutch words from the Dutch-only robot than from the robot that added Turkish translations.</div>
      <p>Children learned new words from both robots: on every test they picked the right picture well above chance. Right after the lesson, they got 66% of Robin's words right and 62% of Deniz's. A week later, both were at 69%. Once the analysis took into account how many times each child heard each word, children did better on Robin's words on both tests.</p>
    </div>
  </div>
</div>
<div class="rat-ch f2" id="rat-ch2" data-guess>
  <div class="rat-chn">2</div>
  <div class="rat-chb">
    <div class="rat-chk">Prediction 2</div>
    <h3 class="rat-cht">Children will prefer the bilingual robot.</h3>
    <div class="rat-guess">
      <p class="rat-gq">After both lessons, each child was asked: “Which robot do you want to play with again?” What would you pick?</p>
      <div class="rat-gb"><button type="button" data-g="robin" data-msg="You picked like 19 of the 67 children. Most chose Deniz."><i></i>Robin</button><button type="button" data-g="deniz" data-msg="You picked like most children: 48 of 67 chose Deniz."><i></i>Deniz</button></div>
      <div class="rat-pref">
        <div class="rat-dots" role="img" aria-label="48 of 67 children chose Deniz, 19 chose Robin"><i class="d" style="--i:0"></i><i class="d" style="--i:1"></i><i class="d" style="--i:2"></i><i class="d" style="--i:3"></i><i class="d" style="--i:4"></i><i class="d" style="--i:5"></i><i class="d" style="--i:6"></i><i class="d" style="--i:7"></i><i class="d" style="--i:8"></i><i class="d" style="--i:9"></i><i class="d" style="--i:10"></i><i class="d" style="--i:11"></i><i class="d" style="--i:12"></i><i class="d" style="--i:13"></i><i class="d" style="--i:14"></i><i class="d" style="--i:15"></i><i class="d" style="--i:16"></i><i class="d" style="--i:17"></i><i class="d" style="--i:18"></i><i class="d" style="--i:19"></i><i class="d" style="--i:20"></i><i class="d" style="--i:21"></i><i class="d" style="--i:22"></i><i class="d" style="--i:23"></i><i class="d" style="--i:24"></i><i class="d" style="--i:25"></i><i class="d" style="--i:26"></i><i class="d" style="--i:27"></i><i class="d" style="--i:28"></i><i class="d" style="--i:29"></i><i class="d" style="--i:30"></i><i class="d" style="--i:31"></i><i class="d" style="--i:32"></i><i class="d" style="--i:33"></i><i class="d" style="--i:34"></i><i class="d" style="--i:35"></i><i class="d" style="--i:36"></i><i class="d" style="--i:37"></i><i class="d" style="--i:38"></i><i class="d" style="--i:39"></i><i class="d" style="--i:40"></i><i class="d" style="--i:41"></i><i class="d" style="--i:42"></i><i class="d" style="--i:43"></i><i class="d" style="--i:44"></i><i class="d" style="--i:45"></i><i class="d" style="--i:46"></i><i class="d" style="--i:47"></i><i class="r" style="--i:48"></i><i class="r" style="--i:49"></i><i class="r" style="--i:50"></i><i class="r" style="--i:51"></i><i class="r" style="--i:52"></i><i class="r" style="--i:53"></i><i class="r" style="--i:54"></i><i class="r" style="--i:55"></i><i class="r" style="--i:56"></i><i class="r" style="--i:57"></i><i class="r" style="--i:58"></i><i class="r" style="--i:59"></i><i class="r" style="--i:60"></i><i class="r" style="--i:61"></i><i class="r" style="--i:62"></i><i class="r" style="--i:63"></i><i class="r" style="--i:64"></i><i class="r" style="--i:65"></i><i class="r" style="--i:66"></i></div>
        <div class="rat-prefkey"><div class="d"><b>48</b> chose Deniz</div><div class="r"><b>19</b> chose Robin</div></div>
      </div>
      <p class="rat-gmsg"></p>
    </div>
    <div class="rat-after">
      <div class="rat-verdict yes"><b>✓</b>Supported. 72% chose Deniz.</div>
      <div class="rat-find"><span>Finding 2</span>Most children preferred the bilingual robot, but their preference did not change how much they learned.</div>
      <div class="rat-gap">
        <div class="d"><span>Liked more</span><b>Deniz</b></div>
        <div class="r"><span>Learned more from</span><b>Robin</b></div>
      </div>
    </div>
  </div>
</div>
<div class="rat-ch f3" id="rat-ch3">
  <div class="rat-chn">3</div>
  <div class="rat-chb">
    <div class="rat-chk">Open question</div>
    <h3 class="rat-cht">Does what children already know change the result?</h3>
    <p>A week after the lesson, children also took standard vocabulary tests in Turkish and in Dutch.</p>
    <div class="rat-verdict yes"><b>✓</b>Yes, with both robots.</div>
    <div class="rat-find"><span>Finding 3</span>Children who already knew more words, in Turkish or in Dutch, learned more from both robots.</div>
    <p>The study found no sign that translations helped children with smaller vocabularies more.</p>
  </div>
</div>
<div class="rat-whyx">
  <h3 class="rat-whyh">So why might translations not help?</h3>
  <div class="rat-reasons">
    <div><b>1</b><strong>Surprise</strong><p>Turkish is rarely heard in Dutch classrooms, and children were often surprised by it.</p></div>
    <div><b>2</b><strong>Extra effort</strong><p>Switching between two languages may have added extra mental effort.</p></div>
    <div><b>3</b><strong>Distraction</strong><p>Excitement about the bilingual robot may have distracted children from learning.</p></div>
  </div>
  <p class="rat-whynote">These are possible explanations, not tested results.</p>
</div>
<div class="rat-part"><span>Part three</span>What it means for products</div>
<div class="rat-biz">
  <div class="rat-bcard f1"><span>Finding 1</span><b>Children learned more Dutch words from the Dutch-only robot than from the robot that added Turkish translations.</b><p>For products: a feature that sounds helpful can reduce learning. Test it before assuming it helps.</p></div>
  <div class="rat-bcard f2"><span>Finding 2</span><b>Most children preferred the bilingual robot, but their preference did not change how much they learned.</b><p>For products: measure preference and performance separately. A well-liked feature is not necessarily an effective one.</p></div>
  <div class="rat-bcard f3"><span>Finding 3</span><b>Children who already knew more words, in Turkish or in Dutch, learned more from both robots.</b><p>For products: users' starting points shape outcomes, so evaluate a feature across users with different levels of prior knowledge.</p></div>
</div>
<div class="rat-take">
  <div class="rat-k">The takeaway</div>
  <p>Children liked the bilingual robot more, but learned more from the Dutch-only robot. Liking a feature and learning from it are different outcomes, so measure both.</p>
</div>
<div class="rat-actions">
  <a class="rat-btn" href="/academia/">Full write-ups &amp; citations</a>
  <a class="rat-btn alt" href="https://doi.org/10.1111/jcal.12510" target="_blank" rel="noopener">Read the paper (open access)</a>
</div>
</div>
<script>
(function () {
  var root = document.querySelector(".rat");
  if (!root) { return; }

  var anims = [].slice.call(root.querySelectorAll("[data-anim]"));
  if ("IntersectionObserver" in window) {
    var io = new IntersectionObserver(function (es) {
      es.forEach(function (e) {
        if (e.isIntersecting) { e.target.classList.add("rat-in"); io.unobserve(e.target); }
      });
    }, { threshold: 0.35 });
    anims.forEach(function (a) { io.observe(a); });
  } else {
    anims.forEach(function (a) { a.classList.add("rat-in"); });
  }

  [].forEach.call(root.querySelectorAll(".rat-ch[data-guess]"), function (ch) {
    var msg = ch.querySelector(".rat-gmsg");
    [].forEach.call(ch.querySelectorAll(".rat-gb button"), function (b) {
      b.addEventListener("click", function () {
        if (ch.hasAttribute("data-g")) { return; }
        ch.setAttribute("data-g", b.getAttribute("data-g"));
        msg.textContent = b.getAttribute("data-msg");
        setTimeout(function () {
          [].forEach.call(ch.querySelectorAll(".rat-plot, .rat-pref"), function (x) { x.classList.add("rat-in"); });
        }, 250);
      });
    });
  });

  var test = document.getElementById("rat-test");
  if (test) {
    var tmsg = document.getElementById("rat-tmsg");
    [].forEach.call(test.querySelectorAll(".rat-tcards button"), function (b) {
      b.addEventListener("click", function () {
        [].forEach.call(test.querySelectorAll(".rat-tcards button"), function (x) { x.classList.remove("ok", "no"); });
        void b.offsetWidth;
        if (b.getAttribute("data-ok") === "1") {
          b.classList.add("ok");
          tmsg.textContent = "Correct! Klappen means clapping.";
        } else {
          b.classList.add("no");
          tmsg.textContent = "Not this one. Try again.";
        }
      });
    });
  }

  var L = document.getElementById("rat-lesson");
  if (!L) { return; }
  var bub = document.getElementById("rat-bub");
  var tbub = document.getElementById("rat-tbub");
  var you = document.getElementById("rat-you");
  var hint = document.getElementById("rat-hint");
  var go = document.getElementById("rat-go");
  var toys = document.getElementById("rat-toys");
  var nameEl = document.getElementById("rat-name");
  var bot = L.querySelector(".rat-bot");

  var words = [
    { an: "monkey", nl: "schudden", tr: "sallamak", verb: "shake",
      find: ["Hey, look! I see a monkey. The monkey is shaking the tree. Touch the monkey that is shaking the tree.",
             "Look! Do you see the monkey that is shaking the tree? In Turkish we say {tr}. Touch the monkey on the screen."],
      tab: "{nl}. The monkey is shaking.",
      act: "Can you shake the toys? Show me how you can shake them." },
    { an: "bear", nl: "klappen", tr: "alkışlamak", verb: "clap",
      find: ["Hey, look! I see a bear. The bear is clapping. Touch the bear that is clapping.",
             "Look! Do you see the bear that is clapping? In Turkish we say {tr}. Touch the bear on the screen."],
      tab: "{nl}. The bear is clapping.",
      act: "Can you make the toys clap? Show me how they can clap." }
  ];
  var sayLine = ["Did you hear that? In Dutch we say {nl}. Say after me: {nl}.",
                 "Oh, so it is {tr} in Turkish and {nl} in Dutch. Say after me: {nl}."];
  var doneLine = "Okay, let's put them back in the bag.";

  var wi = 0;
  var timers = [];
  function later(fn, ms) { timers.push(setTimeout(fn, ms)); }
  function clearTimers() { timers.forEach(clearTimeout); timers = []; }
  function cap(s) { return s.charAt(0).toUpperCase() + s.slice(1); }
  function fill(s, w) {
    return s.replace(/\{tr\}/g, '<b class="tr">' + w.tr + "</b>")
            .replace(/^\{nl\}\./, '<b class="nl">' + cap(w.nl) + "</b>.")
            .replace(/\{nl\}/g, '<b class="nl">' + w.nl + "</b>");
  }
  function ri() { return L.getAttribute("data-r") === "deniz" ? 1 : 0; }
  function step(n) { L.setAttribute("data-step", String(n)); }
  function speak(html) {
    bub.innerHTML = html;
    L.removeAttribute("data-say");
    void bub.offsetWidth;
    L.setAttribute("data-say", "1");
    L.setAttribute("data-talk", "1");
    later(function () { L.removeAttribute("data-talk"); }, 1500);
  }
  function hush() { L.removeAttribute("data-say"); L.removeAttribute("data-talk"); }
  function button(text) {
    if (text) { go.textContent = text; go.hidden = false; } else { go.hidden = true; }
  }

  function reset() {
    clearTimers();
    hush();
    L.removeAttribute("data-you");
    L.removeAttribute("data-happy");
    toys.classList.remove("shake", "clap");
    wi = 0;
    step(0);
    hint.textContent = "Pick a robot, then start.";
    button("Start the lesson");
  }
  function startWord() {
    var w = words[wi];
    clearTimers();
    L.removeAttribute("data-you");
    toys.classList.remove("shake", "clap");
    step(1);
    speak(fill(w.find[ri()], w));
    hint.textContent = "Tap the " + w.an + " on the tablet.";
    button("");
  }
  function tapAnimal(el) {
    if (L.getAttribute("data-step") !== "1") { return; }
    var w = words[wi];
    if (el.getAttribute("data-an") !== w.an) {
      el.classList.remove("rat-no");
      void el.getBoundingClientRect();
      el.classList.add("rat-no");
      return;
    }
    hush();
    tbub.innerHTML = fill(w.tab, w);
    step(2);
    hint.textContent = "Listen to the tablet.";
    later(function () {
      step(3);
      speak(fill(sayLine[ri()], w));
      hint.textContent = "Say the Dutch word.";
      button("Say “" + w.nl + "”");
    }, 1900);
  }
  function sayWord() {
    var w = words[wi];
    you.innerHTML = 'You: “<b class="nl">' + cap(w.nl) + '</b>!”';
    L.setAttribute("data-you", "1");
    L.setAttribute("data-happy", "1");
    hush();
    button("");
    later(function () { L.removeAttribute("data-happy"); }, 600);
    later(function () {
      step(4);
      speak(w.act);
      hint.textContent = "Tap your toys to " + w.verb + " them.";
    }, 900);
  }
  function playToys() {
    if (L.getAttribute("data-step") !== "4") { return; }
    var w = words[wi];
    step(5);
    hush();
    toys.classList.add(w.verb);
    later(function () {
      toys.classList.remove(w.verb);
      speak(doneLine);
      if (wi < words.length - 1) {
        hint.textContent = "Children learned six words this way, three with each robot.";
        button("Next word");
      } else {
        hint.textContent = "That's the lesson. Now switch robots and compare.";
        button("Start again");
      }
    }, 1500);
  }

  go.addEventListener("click", function () {
    var s = L.getAttribute("data-step");
    if (s === "0") { wi = 0; startWord(); }
    else if (s === "3") { sayWord(); }
    else if (s === "5") {
      if (wi < words.length - 1) { wi += 1; startWord(); } else { reset(); }
    }
  });
  [].forEach.call(L.querySelectorAll(".rat-an"), function (el) {
    el.addEventListener("click", function () { tapAnimal(el); });
    el.addEventListener("keydown", function (e) {
      if (e.key === "Enter" || e.key === " ") { e.preventDefault(); tapAnimal(el); }
    });
  });
  toys.addEventListener("click", playToys);
  toys.addEventListener("keydown", function (e) {
    if (e.key === "Enter" || e.key === " ") { e.preventDefault(); playToys(); }
  });
  [].forEach.call(L.querySelectorAll(".rat-pick button"), function (b) {
    b.addEventListener("click", function () {
      [].forEach.call(L.querySelectorAll(".rat-pick button"), function (x) {
        x.classList.toggle("on", x === b);
        x.setAttribute("aria-pressed", x === b ? "true" : "false");
      });
      L.setAttribute("data-r", b.getAttribute("data-r"));
      nameEl.textContent = b.getAttribute("data-r") === "deniz" ? "Deniz" : "Robin";
      reset();
    });
  });

  var pupils = [].slice.call(bot.querySelectorAll(".pupil"));
  function gaze(x, y) {
    pupils.forEach(function (p) { p.style.transform = "translate(" + x + "px," + y + "px)"; });
  }
  function glance() {
    var spots = [[-3.5, -1], [3.5, -1], [-3, 2], [3, 2], [0, -3], [2, 0]];
    var d = spots[Math.floor(Math.random() * spots.length)];
    if (Math.random() < 0.25) { gaze((Math.random() - 0.5) * 1.2, (Math.random() - 0.5) * 1.2); } else { gaze(d[0], d[1]); }
    setTimeout(function () { gaze(0, 0); }, 500 + Math.random() * 900);
    setTimeout(glance, 2200 + Math.random() * 3800);
  }
  gaze(0, 0);
  setTimeout(glance, 2500);
})();
</script>
