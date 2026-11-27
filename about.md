---
title: About
permalink: /about/
layout: page
excerpt: Who's asking? A UX and behavioral researcher explains herself four ways, and what that has to do with audience design.
comments: false
---
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Figtree:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<style>
.header:has(+ .page-content .abt){display:none}
.abt{--ink:#1d1b26;--muted:#6a6878;--card:#f5f2ec;--card2:#ebe6dd;--me:#ffffff;--line:rgba(29,27,38,.1);--rec:#3b6fe0;--rec-s:#dce6fb;--fr:#e8603f;--fr-s:#fbe0d8;--kid:#e8a514;--kid-s:#fbedc8;--bot:#13a184;--bot-s:#d3f0e8;--c:var(--rec);--cs:var(--rec-s)}
body[data-theme="dark"] .abt{--ink:#efece6;--muted:#a6a3b0;--card:#24232c;--card2:#2e2d38;--me:#33323e;--line:rgba(255,255,255,.1);--rec:#7aa2ff;--rec-s:#2b3a5e;--fr:#ff8f72;--fr-s:#55332d;--kid:#ffc857;--kid-s:#524425;--bot:#3fd3b1;--bot-s:#1f4a42}
.abt[data-l="fr"]{--c:var(--fr);--cs:var(--fr-s)}
.abt[data-l="kid"]{--c:var(--kid);--cs:var(--kid-s)}
.abt[data-l="bot"]{--c:var(--bot);--cs:var(--bot-s)}
.abt{font-family:"Figtree",system-ui,-apple-system,"Segoe UI",sans-serif;color:var(--ink);font-size:16.5px;line-height:1.55;padding:6px 0 30px}
.abt *{box-sizing:border-box}
.abt p{margin:0}
.abt button{font-family:inherit;cursor:pointer}
.abt .av{display:block;border-radius:50%}
.abt p.abt-kick{font-size:13px;font-weight:700;letter-spacing:.14em;text-transform:uppercase;color:var(--muted);margin-bottom:6px}
.abt h1.abt-title{font-family:inherit;font-size:clamp(44px,9vw,72px);font-weight:800;line-height:1;letter-spacing:-.03em;margin:0 0 16px;color:var(--ink)}
.abt .abt-qm{color:var(--c);display:inline-block;transition:color .35s,transform .35s}
.abt .abt-qm.abt-pop{animation:abtpop .45s}
@keyframes abtpop{40%{transform:rotate(14deg) scale(1.15)}}
.abt p.abt-lead{font-size:19px;color:var(--ink);max-width:560px;margin-bottom:26px}
.abt-stage{background:var(--card);border-radius:22px;padding:22px 22px 18px}
.abt p.abt-step{font-size:14px;font-weight:700;color:var(--muted);margin:0 0 10px;display:flex;align-items:center;gap:8px}
.abt p.abt-step span{width:22px;height:22px;border-radius:50%;background:var(--ink);color:var(--card);font-size:12px;display:inline-flex;align-items:center;justify-content:center}
.abt-who{display:grid;grid-template-columns:repeat(4,1fr);gap:10px;margin-bottom:20px}
.abt .abt-l{background:var(--me);border:2px solid transparent;border-radius:16px;padding:12px 6px 10px;display:flex;flex-direction:column;align-items:center;gap:7px;color:var(--ink);transition:transform .2s,border-color .2s,box-shadow .2s}
.abt .abt-l .av-b{width:58px;height:58px;transition:transform .25s}
.abt .abt-l:hover .av-b{transform:translateY(-3px)}
.abt .abt-ln{font-size:14.5px;font-weight:600}
.abt .abt-l[data-l="rec"][aria-pressed="true"]{border-color:var(--rec)}
.abt .abt-l[data-l="fr"][aria-pressed="true"]{border-color:var(--fr)}
.abt .abt-l[data-l="kid"][aria-pressed="true"]{border-color:var(--kid)}
.abt .abt-l[data-l="bot"][aria-pressed="true"]{border-color:var(--bot)}
.abt .abt-l[aria-pressed="true"]{box-shadow:0 6px 16px -10px rgba(0,0,0,.45);transform:translateY(-2px)}
.abt .abt-l[aria-pressed="false"] .av-b{filter:saturate(.75)}
.abt-qs{display:flex;flex-wrap:wrap;gap:8px;margin-bottom:18px}
.abt .abt-q{border:0;background:var(--card2);color:var(--ink);font-size:15px;font-weight:600;padding:8px 15px;border-radius:999px;transition:background .2s,color .2s}
.abt .abt-q:hover{background:var(--cs)}
.abt .abt-q[aria-pressed="true"]{background:var(--ink);color:var(--card)}
.abt .abt-l:focus-visible,.abt .abt-q:focus-visible,.abt .abt-hl:focus-visible{outline:3px solid var(--c);outline-offset:2px}
.abt-log{display:flex;flex-direction:column;gap:12px;min-height:230px;padding:16px;border-radius:16px;background:var(--me);margin-bottom:16px}
.abt-row{display:flex;align-items:flex-end;gap:9px}
.abt-them{flex-direction:row-reverse}
.abt .abt-a{width:36px;height:36px;border-radius:50%;flex:0 0 36px;object-fit:cover;display:block}
.abt img.abt-a{margin:0!important;max-width:none}
.abt .abt-a .av{width:36px;height:36px}
.abt p.abt-b,.abt div.abt-b{max-width:82%;padding:10px 14px;border-radius:18px;font-size:16px;line-height:1.5}
.abt p.abt-ask,.abt p.abt-rb{background:var(--c);color:#fff;border-bottom-right-radius:5px;font-weight:500}
body[data-theme="dark"] .abt p.abt-ask,body[data-theme="dark"] .abt p.abt-rb{color:#17161d}
.abt div.abt-ans{background:var(--card);border-bottom-left-radius:5px;min-width:64px}
.abt-re{opacity:0;transform:translateY(6px);transition:opacity .3s,transform .3s}
.abt-re.abt-on{opacity:1;transform:none}
.abt-dots{display:none;gap:4px;padding:5px 2px}
.abt-ans.abt-typing .abt-dots{display:inline-flex}
.abt-ans.abt-typing .abt-txt{display:none}
.abt-dots i{width:7px;height:7px;border-radius:50%;background:var(--muted);animation:abtdot 1s infinite}
.abt-dots i:nth-child(2){animation-delay:.15s}
.abt-dots i:nth-child(3){animation-delay:.3s}
@keyframes abtdot{0%,60%,100%{opacity:.25;transform:none}30%{opacity:1;transform:translateY(-3px)}}
.abt .abt-w{opacity:0;transition:opacity .18s}
.abt .abt-txt.abt-show .abt-w{opacity:1}
.abt .abt-u{border-radius:4px;transition:background .25s,box-shadow .25s}
.abt.abt-hlon .abt-u{background:var(--cs);box-shadow:0 0 0 2px var(--cs)}
.abt .abt-line{display:block}
.abt .abt-line+.abt-line{margin-top:3px}
.abt .abt-lab{display:inline-block;font-size:11.5px;font-weight:700;letter-spacing:.08em;text-transform:uppercase;background:var(--bot);color:#fff;border-radius:5px;padding:1px 6px;margin-right:6px;vertical-align:1px}
body[data-theme="dark"] .abt .abt-lab{color:#17161d}
.abt .abt-line.abt-end{color:var(--muted);font-weight:600}
.abt-mh{display:flex;align-items:center;justify-content:space-between;gap:10px;margin-bottom:10px;flex-wrap:wrap}
.abt p.abt-mtl{font-size:14px;font-weight:700;color:var(--muted)}
.abt .abt-hl{border:2px solid var(--ink);background:transparent;color:var(--ink);font-size:13.5px;font-weight:700;padding:4px 12px;border-radius:999px}
.abt .abt-hl[aria-pressed="true"]{background:var(--ink);color:var(--card)}
.abt-mr{display:grid;grid-template-columns:24px 92px 1fr 26px;align-items:center;gap:9px;padding:4px 0;opacity:.55;transition:opacity .25s}
.abt-mr.abt-cur{opacity:1}
.abt .abt-mr .av-m{width:24px;height:24px}
.abt .abt-mn{font-size:14px;font-weight:600}
.abt .abt-mt{height:12px;border-radius:999px;background:var(--card2);overflow:hidden}
.abt .abt-mb{display:block;height:100%;width:0;border-radius:999px;transition:width .6s cubic-bezier(.3,.9,.3,1)}
.abt-mr[data-l="rec"] .abt-mb{background:var(--rec)}
.abt-mr[data-l="fr"] .abt-mb{background:var(--fr)}
.abt-mr[data-l="kid"] .abt-mb{background:var(--kid)}
.abt-mr[data-l="bot"] .abt-mb{background:var(--bot)}
.abt .abt-mv{font-size:15px;font-weight:800;text-align:right;font-variant-numeric:tabular-nums}
.abt-mr.abt-cur .abt-mn{font-weight:800}
.abt p.abt-mnote{font-size:13.5px;color:var(--muted);margin-top:10px;line-height:1.45}
.abt-def{margin-top:52px}
.abt h2.abt-h2{font-family:inherit;font-size:clamp(28px,5vw,38px);font-weight:800;letter-spacing:-.02em;line-height:1.12;margin:0 0 14px;color:var(--ink)}
.abt .abt-mark{background:linear-gradient(transparent 58%,var(--cs) 58%);padding:0 3px;transition:background .35s}
.abt p.abt-p{font-size:17px;max-width:600px}
.abt-three{display:grid;grid-template-columns:repeat(3,1fr);gap:12px;margin:22px 0 14px}
.abt-c{background:var(--card);border-radius:16px;padding:16px 16px 18px}
.abt .abt-cn{display:inline-flex;width:26px;height:26px;border-radius:8px;align-items:center;justify-content:center;font-weight:800;font-size:14px;background:var(--ink);color:var(--card);margin-bottom:10px}
.abt p.abt-ct{font-weight:700;font-size:16px;line-height:1.3;margin-bottom:6px}
.abt p.abt-cp{font-size:15px;color:var(--muted);line-height:1.45}
.abt p.abt-src{font-size:13.5px;color:var(--muted)}
.abt-why{margin-top:44px;display:grid;grid-template-columns:96px 1fr;gap:20px;align-items:start;background:var(--bot-s);border-radius:22px;padding:24px}
.abt .abt-whyav .av-w{width:96px;height:96px}
.abt .av-eyes{transform-origin:center;transform-box:fill-box;animation:abtblink 4.5s infinite}
@keyframes abtblink{0%,92%,100%{transform:scaleY(1)}95%{transform:scaleY(.12)}}
.abt p.abt-go{display:flex;flex-wrap:wrap;gap:10px;margin-top:16px}
.abt p.abt-go a,.abt p.abt-out a{display:inline-flex;align-items:center;gap:6px;font-weight:700;font-size:15px;text-decoration:none!important;border-radius:999px;padding:8px 16px;transition:transform .2s}
.abt p.abt-go a{background:var(--ink);color:var(--card)!important}
.abt p.abt-go a:hover,.abt p.abt-out a:hover{transform:translateY(-2px)}
.abt p.abt-out{display:flex;flex-wrap:wrap;gap:10px;margin-top:34px;justify-content:center}
.abt p.abt-out a{border:2px solid var(--line);color:var(--ink)!important;background:transparent}
.abt p.abt-out a:hover{border-color:var(--ink)}
@media (max-width:600px){
.abt-stage{padding:16px 12px 14px;border-radius:18px}
.abt-who{gap:6px}
.abt .abt-l{padding:9px 2px 8px;border-radius:13px}
.abt .abt-l .av-b{width:46px;height:46px}
.abt .abt-ln{font-size:12.5px}
.abt-qs{gap:6px}
.abt .abt-q{font-size:14px;padding:7px 11px}
.abt-log{padding:12px 10px;min-height:260px}
.abt p.abt-b,.abt div.abt-b{max-width:88%;font-size:15.5px}
.abt-mr{grid-template-columns:22px 80px 1fr 22px;gap:7px}
.abt-three{grid-template-columns:1fr}
.abt-why{grid-template-columns:1fr;padding:20px}
.abt .abt-whyav .av-w{width:72px;height:72px}
}
@media (prefers-reduced-motion:reduce){.abt *{animation:none!important;transition:none!important}}
</style>
<div class="abt" data-l="rec">
<p class="abt-kick">About</p>
<h1 class="abt-title">Who’s asking<span class="abt-qm">?</span></h1>
<p class="abt-lead">How I describe myself depends on who’s listening. So does yours. Pick who’s asking, then pick a question, and watch the answer change.</p>
<div class="abt-stage">
<p class="abt-step"><span>1</span>Who’s asking?</p>
<div class="abt-who"><button type="button" class="abt-l" data-l="rec" aria-pressed="true"><svg class="av av-b" viewBox="0 0 64 64" aria-hidden="true"><circle cx="32" cy="32" r="32" style="fill:var(--rec-s)"/><path d="M10 64C10 51 20 44 32 44C44 44 54 51 54 64Z" style="fill:var(--rec)"/><path d="M26 44.5L32 53L38 44.5Z" fill="#fff"/><path d="M30.6 47.5L33.4 47.5L34.4 58L32 61L29.6 58Z" fill="#1d1b26"/><rect x="29" y="35" width="6" height="10" fill="#e8b48f"/><circle cx="32" cy="27" r="11" fill="#e8b48f"/><path d="M21 26C20 16 27 12.5 33 13C40 13.5 44 18 43 25C40 20 34 19 28 21C25 22 23 24 21 26Z" fill="#2b2333"/><g fill="none" stroke="#1d1b26" stroke-width="1.4"><circle cx="27.6" cy="28" r="3.2"/><circle cx="36.4" cy="28" r="3.2"/><path d="M30.8 28L33.2 28"/></g><path d="M29.5 33.2Q32 34.4 34.5 33.2" fill="none" stroke="#1d1b26" stroke-width="1.3" stroke-linecap="round"/></svg><span class="abt-ln">Recruiter</span></button><button type="button" class="abt-l" data-l="fr" aria-pressed="false"><svg class="av av-b" viewBox="0 0 64 64" aria-hidden="true"><circle cx="32" cy="32" r="32" style="fill:var(--fr-s)"/><path d="M19 30C18 16 25 12 32 12C40 12 46 17 45 30L46 46L18 46Z" fill="#6b3a28"/><path d="M10 64C10 51 20 44 32 44C44 44 54 51 54 64Z" style="fill:var(--fr)"/><rect x="29" y="35" width="6" height="10" fill="#f3cfae"/><circle cx="32" cy="27" r="11" fill="#f3cfae"/><path d="M21 26C22 16 30 13 36 15C41 17 43 21 43 26C37 23 31 21 27.5 18C25.5 21 23.5 23.5 21 26Z" fill="#6b3a28"/><circle cx="28" cy="27.8" r="1.3" fill="#1d1b26"/><circle cx="36" cy="27.8" r="1.3" fill="#1d1b26"/><path d="M28 31.6Q32 35.6 36 31.6" fill="none" stroke="#1d1b26" stroke-width="1.5" stroke-linecap="round"/></svg><span class="abt-ln">Friend</span></button><button type="button" class="abt-l" data-l="kid" aria-pressed="false"><svg class="av av-b" viewBox="0 0 64 64" aria-hidden="true"><circle cx="32" cy="32" r="32" style="fill:var(--kid-s)"/><circle cx="17" cy="27" r="6" fill="#2b2333"/><circle cx="47" cy="27" r="6" fill="#2b2333"/><path d="M16 64C16 54 23 49 32 49C41 49 48 54 48 64Z" style="fill:var(--kid)"/><rect x="29" y="40" width="6" height="10" fill="#c98d66"/><circle cx="32" cy="30" r="13" fill="#c98d66"/><path d="M19 29C19 19 26 15.5 32 15.5C39 15.5 45 19.5 45 29C40 24.5 35.5 22.5 32 22.5C28 22.5 23.5 24.5 19 29Z" fill="#2b2333"/><circle cx="27" cy="30.5" r="1.7" fill="#1d1b26"/><circle cx="37" cy="30.5" r="1.7" fill="#1d1b26"/><circle cx="24" cy="35" r="2.2" fill="#ff8f7d" opacity=".55"/><circle cx="40" cy="35" r="2.2" fill="#ff8f7d" opacity=".55"/><path d="M27.5 35Q32 40 36.5 35Z" fill="#1d1b26"/></svg><span class="abt-ln">5-year-old</span></button><button type="button" class="abt-l" data-l="bot" aria-pressed="false"><svg class="av av-b" viewBox="0 0 64 64" aria-hidden="true"><circle cx="32" cy="32" r="32" style="fill:var(--bot-s)"/><rect x="17" y="48" width="30" height="20" rx="7" style="fill:var(--bot)"/><rect x="29" y="41" width="6" height="8" fill="#9aa7ad"/><path d="M32 18L32 11" stroke="#9aa7ad" stroke-width="2"/><circle cx="32" cy="9.5" r="3.2" style="fill:var(--bot)"/><rect x="12.5" y="25" width="4.5" height="10" rx="2" fill="#9aa7ad"/><rect x="47" y="25" width="4.5" height="10" rx="2" fill="#9aa7ad"/><rect x="16" y="17" width="32" height="25" rx="9" fill="#eef2f3" stroke="#c5cfd3" stroke-width="1"/><g class="av-eyes"><circle cx="26" cy="29" r="4" fill="#1d1b26"/><circle cx="38" cy="29" r="4" fill="#1d1b26"/><circle cx="27.4" cy="27.6" r="1.2" fill="#fff"/><circle cx="39.4" cy="27.6" r="1.2" fill="#fff"/></g><path d="M28 36.5L36 36.5" stroke="#1d1b26" stroke-width="1.6" stroke-linecap="round"/></svg><span class="abt-ln">Robot</span></button></div>
<p class="abt-step"><span>2</span>What do they want to know?</p>
<div class="abt-qs"><button type="button" class="abt-q" data-q="0" aria-pressed="true">What I do</button><button type="button" class="abt-q" data-q="1" aria-pressed="false">How I got here</button><button type="button" class="abt-q" data-q="2" aria-pressed="false">What’s next</button></div>
<div class="abt-log" aria-live="polite">
<div class="abt-row abt-them"><span class="abt-a abt-la"></span><p class="abt-b abt-ask"></p></div>
<div class="abt-row abt-me"><img class="abt-a" src="{{ site.author.avatar }}" alt="Hande"><div class="abt-b abt-ans"><span class="abt-dots"><i></i><i></i><i></i></span><div class="abt-txt"></div></div></div>
<div class="abt-row abt-them abt-re"><span class="abt-a abt-la"></span><p class="abt-b abt-rb"></p></div>
</div>
<div class="abt-meter">
<div class="abt-mh"><p class="abt-mtl">Pieces of information in each answer</p><button type="button" class="abt-hl" aria-pressed="false">Highlight them</button></div>
<div class="abt-mr" data-l="rec"><svg class="av av-m" viewBox="0 0 64 64" aria-hidden="true"><circle cx="32" cy="32" r="32" style="fill:var(--rec-s)"/><path d="M10 64C10 51 20 44 32 44C44 44 54 51 54 64Z" style="fill:var(--rec)"/><path d="M26 44.5L32 53L38 44.5Z" fill="#fff"/><path d="M30.6 47.5L33.4 47.5L34.4 58L32 61L29.6 58Z" fill="#1d1b26"/><rect x="29" y="35" width="6" height="10" fill="#e8b48f"/><circle cx="32" cy="27" r="11" fill="#e8b48f"/><path d="M21 26C20 16 27 12.5 33 13C40 13.5 44 18 43 25C40 20 34 19 28 21C25 22 23 24 21 26Z" fill="#2b2333"/><g fill="none" stroke="#1d1b26" stroke-width="1.4"><circle cx="27.6" cy="28" r="3.2"/><circle cx="36.4" cy="28" r="3.2"/><path d="M30.8 28L33.2 28"/></g><path d="M29.5 33.2Q32 34.4 34.5 33.2" fill="none" stroke="#1d1b26" stroke-width="1.3" stroke-linecap="round"/></svg><span class="abt-mn">Recruiter</span><span class="abt-mt"><span class="abt-mb"></span></span><span class="abt-mv">0</span></div><div class="abt-mr" data-l="fr"><svg class="av av-m" viewBox="0 0 64 64" aria-hidden="true"><circle cx="32" cy="32" r="32" style="fill:var(--fr-s)"/><path d="M19 30C18 16 25 12 32 12C40 12 46 17 45 30L46 46L18 46Z" fill="#6b3a28"/><path d="M10 64C10 51 20 44 32 44C44 44 54 51 54 64Z" style="fill:var(--fr)"/><rect x="29" y="35" width="6" height="10" fill="#f3cfae"/><circle cx="32" cy="27" r="11" fill="#f3cfae"/><path d="M21 26C22 16 30 13 36 15C41 17 43 21 43 26C37 23 31 21 27.5 18C25.5 21 23.5 23.5 21 26Z" fill="#6b3a28"/><circle cx="28" cy="27.8" r="1.3" fill="#1d1b26"/><circle cx="36" cy="27.8" r="1.3" fill="#1d1b26"/><path d="M28 31.6Q32 35.6 36 31.6" fill="none" stroke="#1d1b26" stroke-width="1.5" stroke-linecap="round"/></svg><span class="abt-mn">Friend</span><span class="abt-mt"><span class="abt-mb"></span></span><span class="abt-mv">0</span></div><div class="abt-mr" data-l="kid"><svg class="av av-m" viewBox="0 0 64 64" aria-hidden="true"><circle cx="32" cy="32" r="32" style="fill:var(--kid-s)"/><circle cx="17" cy="27" r="6" fill="#2b2333"/><circle cx="47" cy="27" r="6" fill="#2b2333"/><path d="M16 64C16 54 23 49 32 49C41 49 48 54 48 64Z" style="fill:var(--kid)"/><rect x="29" y="40" width="6" height="10" fill="#c98d66"/><circle cx="32" cy="30" r="13" fill="#c98d66"/><path d="M19 29C19 19 26 15.5 32 15.5C39 15.5 45 19.5 45 29C40 24.5 35.5 22.5 32 22.5C28 22.5 23.5 24.5 19 29Z" fill="#2b2333"/><circle cx="27" cy="30.5" r="1.7" fill="#1d1b26"/><circle cx="37" cy="30.5" r="1.7" fill="#1d1b26"/><circle cx="24" cy="35" r="2.2" fill="#ff8f7d" opacity=".55"/><circle cx="40" cy="35" r="2.2" fill="#ff8f7d" opacity=".55"/><path d="M27.5 35Q32 40 36.5 35Z" fill="#1d1b26"/></svg><span class="abt-mn">5-year-old</span><span class="abt-mt"><span class="abt-mb"></span></span><span class="abt-mv">0</span></div><div class="abt-mr" data-l="bot"><svg class="av av-m" viewBox="0 0 64 64" aria-hidden="true"><circle cx="32" cy="32" r="32" style="fill:var(--bot-s)"/><rect x="17" y="48" width="30" height="20" rx="7" style="fill:var(--bot)"/><rect x="29" y="41" width="6" height="8" fill="#9aa7ad"/><path d="M32 18L32 11" stroke="#9aa7ad" stroke-width="2"/><circle cx="32" cy="9.5" r="3.2" style="fill:var(--bot)"/><rect x="12.5" y="25" width="4.5" height="10" rx="2" fill="#9aa7ad"/><rect x="47" y="25" width="4.5" height="10" rx="2" fill="#9aa7ad"/><rect x="16" y="17" width="32" height="25" rx="9" fill="#eef2f3" stroke="#c5cfd3" stroke-width="1"/><g class="av-eyes"><circle cx="26" cy="29" r="4" fill="#1d1b26"/><circle cx="38" cy="29" r="4" fill="#1d1b26"/><circle cx="27.4" cy="27.6" r="1.2" fill="#fff"/><circle cx="39.4" cy="27.6" r="1.2" fill="#fff"/></g><path d="M28 36.5L36 36.5" stroke="#1d1b26" stroke-width="1.6" stroke-linecap="round"/></svg><span class="abt-mn">Robot</span><span class="abt-mt"><span class="abt-mb"></span></span><span class="abt-mv">0</span></div>
<p class="abt-mnote">I scored each answer the way I scored descriptions in my studies: one point for every separate, meaningful piece of information.</p>
</div>
</div>
<section class="abt-def">
<p class="abt-kick">The idea behind it</p>
<h2 class="abt-h2">That is <span class="abt-mark">audience design</span>.</h2>
<p class="abt-p">Speakers shape what they say around who they are saying it to. We guess what our listener already knows, what they need, and how much they can take in. Then we adjust our words, how much detail we give, and how explicit we are. Most of the time we do it without noticing.</p>
<div class="abt-three">
<div class="abt-c"><span class="abt-cn">1</span><p class="abt-ct">What do they already know?</p><p class="abt-cp">A recruiter knows what a PhD is. A five-year-old doesn’t.</p></div>
<div class="abt-c"><span class="abt-cn">2</span><p class="abt-ct">What do they need from me?</p><p class="abt-cp">A recruiter needs facts to compare. A friend wants the story.</p></div>
<div class="abt-c"><span class="abt-cn">3</span><p class="abt-ct">Are they following?</p><p class="abt-cp">When a listener looks lost, we say it again, with more detail.</p></div>
</div>
<p class="abt-src">The term comes from linguistics and psychology: Clark &amp; Murphy (1982) and Bell (1984).</p>
</section>
<section class="abt-why">
<div class="abt-whyav"><svg class="av av-w" viewBox="0 0 64 64" aria-hidden="true"><circle cx="32" cy="32" r="32" style="fill:var(--bot-s)"/><rect x="17" y="48" width="30" height="20" rx="7" style="fill:var(--bot)"/><rect x="29" y="41" width="6" height="8" fill="#9aa7ad"/><path d="M32 18L32 11" stroke="#9aa7ad" stroke-width="2"/><circle cx="32" cy="9.5" r="3.2" style="fill:var(--bot)"/><rect x="12.5" y="25" width="4.5" height="10" rx="2" fill="#9aa7ad"/><rect x="47" y="25" width="4.5" height="10" rx="2" fill="#9aa7ad"/><rect x="16" y="17" width="32" height="25" rx="9" fill="#eef2f3" stroke="#c5cfd3" stroke-width="1"/><g class="av-eyes"><circle cx="26" cy="29" r="4" fill="#1d1b26"/><circle cx="38" cy="29" r="4" fill="#1d1b26"/><circle cx="27.4" cy="27.6" r="1.2" fill="#fff"/><circle cx="39.4" cy="27.6" r="1.2" fill="#fff"/></g><path d="M28 36.5L36 36.5" stroke="#1d1b26" stroke-width="1.6" stroke-linecap="round"/></svg></div>
<div>
<h2 class="abt-h2">Why robots?</h2>
<p class="abt-p">With another person, we can make a good guess about what they know. With a robot, it is much harder. That makes robots an interesting test of audience design, and it is what my PhD was about. In my studies, people gave a robot more detail than a human listener. When the robot said it couldn’t find the word, they added even more on their next try.</p>
<p class="abt-go"><a href="/projects/talking-to-robots/">Talking to Robots <span aria-hidden="true">→</span></a><a href="/projects/robots-as-tutors/">Robots as Tutors <span aria-hidden="true">→</span></a></p>
</div>
</section>
<p class="abt-out"><a href="/assets/HS_resume_202611.pdf" target="_blank" rel="noopener">Resume</a><a href="https://linkedin.com/in/{{ site.author.linkedin }}" target="_blank" rel="noopener">LinkedIn</a><a href="mailto:{{ site.author.email }}">Email</a></p>
</div>
<script>
(function(){
var R=document.querySelector('.abt');
if(!R)return;
var D={"ask": {"rec": ["What do you do?", "Walk me through your background.", "What are you looking for next?"], "fr": ["So what do you actually do?", "How did you end up doing that?", "What’s next for you?"], "kid": ["What’s your job?", "How did you get that job?", "What will you do when you grow up?"], "bot": ["Query: occupation.", "Query: history.", "Query: next goal."]}, "ans": {"rec": ["I’m a {UX and behavioral researcher} with a {PhD in Psychology}. I {design controlled user studies}, {run them with participants}, {analyze the data in R}, and turn the results into {findings that designers and engineers can act on}.", "{BA in Psychology}, with a {certificate in Linguistics}, at {Boğaziçi University}. {Research master’s in Language and Communication} at {Radboud University}. {Research assistant at Tilburg University} on {L2TOR}, {an EU project with a robot tutor for children}. Then a {PhD in Psychology at Koç University}, {2020–2026}.", "I’m moving into {UX research}: {usability testing} and {user studies} of {interactive products}, turning what I find into {actionable insights} {for designers and engineers}."], "fr": ["I {study how people talk to robots}. I set up {word-guessing games}, then {count how much detail people give the robot}.", "{Psychology in Istanbul}, then {a master’s in the Netherlands}. There I {worked on a project where a small robot taught children words}. Back in Istanbul, {my PhD looked at how people talk to robots}.", "{Leaving academia} {for UX research}. Same curiosity, {real products}."], "kid": ["I {play guessing games} {with a little robot}!", "I {went to school for a long, long time}, {in two countries}. Then {I started working with robots}.", "I’m already grown up! Now I want to {help make gadgets easier to use}."], "bot": ["Statement: {I am a researcher}.|Subject: {humans} {talking to robots}.|Step 1: {a human describes a word}.|Step 2: {a robot guesses the word}.|Step 3: {I count each piece of information}.|Step 4: {I compare} {robot listeners with human listeners}.|Please confirm you understood.", "Step 1: {psychology}, {Istanbul}, {2016}.|Step 2: {language and communication}, {Nijmegen}, {2018}.|Step 3: {robot tutor project}, {Tilburg}.|Step 4: {PhD}, {Istanbul}, {2026}.|End of sequence. Please confirm you understood.", "Next goal: {UX research}.|Method: {observe users} {using a product}, {find problems}, {report them clearly} {to the people who build it}.|Reason: {products should fit their users}.|Please confirm you understood."]}, "react": {"rec": ["Sounds relevant. Do you have a resume?", "Clear path. Thanks.", "Good to know. Let’s talk."], "fr": ["Wait, we talk to robots differently?", "That’s a lot of moving around!", "Good for you!"], "kid": ["Can I play too?", "That’s sooo long.", "Even the TV remote?"], "bot": ["Understood.", "Sequence stored. Understood.", "Goal logged. Understood."]}, "av": {"rec": "<svg class=\"av av-s\" viewBox=\"0 0 64 64\" aria-hidden=\"true\"><circle cx=\"32\" cy=\"32\" r=\"32\" style=\"fill:var(--rec-s)\"/><path d=\"M10 64C10 51 20 44 32 44C44 44 54 51 54 64Z\" style=\"fill:var(--rec)\"/><path d=\"M26 44.5L32 53L38 44.5Z\" fill=\"#fff\"/><path d=\"M30.6 47.5L33.4 47.5L34.4 58L32 61L29.6 58Z\" fill=\"#1d1b26\"/><rect x=\"29\" y=\"35\" width=\"6\" height=\"10\" fill=\"#e8b48f\"/><circle cx=\"32\" cy=\"27\" r=\"11\" fill=\"#e8b48f\"/><path d=\"M21 26C20 16 27 12.5 33 13C40 13.5 44 18 43 25C40 20 34 19 28 21C25 22 23 24 21 26Z\" fill=\"#2b2333\"/><g fill=\"none\" stroke=\"#1d1b26\" stroke-width=\"1.4\"><circle cx=\"27.6\" cy=\"28\" r=\"3.2\"/><circle cx=\"36.4\" cy=\"28\" r=\"3.2\"/><path d=\"M30.8 28L33.2 28\"/></g><path d=\"M29.5 33.2Q32 34.4 34.5 33.2\" fill=\"none\" stroke=\"#1d1b26\" stroke-width=\"1.3\" stroke-linecap=\"round\"/></svg>", "fr": "<svg class=\"av av-s\" viewBox=\"0 0 64 64\" aria-hidden=\"true\"><circle cx=\"32\" cy=\"32\" r=\"32\" style=\"fill:var(--fr-s)\"/><path d=\"M19 30C18 16 25 12 32 12C40 12 46 17 45 30L46 46L18 46Z\" fill=\"#6b3a28\"/><path d=\"M10 64C10 51 20 44 32 44C44 44 54 51 54 64Z\" style=\"fill:var(--fr)\"/><rect x=\"29\" y=\"35\" width=\"6\" height=\"10\" fill=\"#f3cfae\"/><circle cx=\"32\" cy=\"27\" r=\"11\" fill=\"#f3cfae\"/><path d=\"M21 26C22 16 30 13 36 15C41 17 43 21 43 26C37 23 31 21 27.5 18C25.5 21 23.5 23.5 21 26Z\" fill=\"#6b3a28\"/><circle cx=\"28\" cy=\"27.8\" r=\"1.3\" fill=\"#1d1b26\"/><circle cx=\"36\" cy=\"27.8\" r=\"1.3\" fill=\"#1d1b26\"/><path d=\"M28 31.6Q32 35.6 36 31.6\" fill=\"none\" stroke=\"#1d1b26\" stroke-width=\"1.5\" stroke-linecap=\"round\"/></svg>", "kid": "<svg class=\"av av-s\" viewBox=\"0 0 64 64\" aria-hidden=\"true\"><circle cx=\"32\" cy=\"32\" r=\"32\" style=\"fill:var(--kid-s)\"/><circle cx=\"17\" cy=\"27\" r=\"6\" fill=\"#2b2333\"/><circle cx=\"47\" cy=\"27\" r=\"6\" fill=\"#2b2333\"/><path d=\"M16 64C16 54 23 49 32 49C41 49 48 54 48 64Z\" style=\"fill:var(--kid)\"/><rect x=\"29\" y=\"40\" width=\"6\" height=\"10\" fill=\"#c98d66\"/><circle cx=\"32\" cy=\"30\" r=\"13\" fill=\"#c98d66\"/><path d=\"M19 29C19 19 26 15.5 32 15.5C39 15.5 45 19.5 45 29C40 24.5 35.5 22.5 32 22.5C28 22.5 23.5 24.5 19 29Z\" fill=\"#2b2333\"/><circle cx=\"27\" cy=\"30.5\" r=\"1.7\" fill=\"#1d1b26\"/><circle cx=\"37\" cy=\"30.5\" r=\"1.7\" fill=\"#1d1b26\"/><circle cx=\"24\" cy=\"35\" r=\"2.2\" fill=\"#ff8f7d\" opacity=\".55\"/><circle cx=\"40\" cy=\"35\" r=\"2.2\" fill=\"#ff8f7d\" opacity=\".55\"/><path d=\"M27.5 35Q32 40 36.5 35Z\" fill=\"#1d1b26\"/></svg>", "bot": "<svg class=\"av av-s\" viewBox=\"0 0 64 64\" aria-hidden=\"true\"><circle cx=\"32\" cy=\"32\" r=\"32\" style=\"fill:var(--bot-s)\"/><rect x=\"17\" y=\"48\" width=\"30\" height=\"20\" rx=\"7\" style=\"fill:var(--bot)\"/><rect x=\"29\" y=\"41\" width=\"6\" height=\"8\" fill=\"#9aa7ad\"/><path d=\"M32 18L32 11\" stroke=\"#9aa7ad\" stroke-width=\"2\"/><circle cx=\"32\" cy=\"9.5\" r=\"3.2\" style=\"fill:var(--bot)\"/><rect x=\"12.5\" y=\"25\" width=\"4.5\" height=\"10\" rx=\"2\" fill=\"#9aa7ad\"/><rect x=\"47\" y=\"25\" width=\"4.5\" height=\"10\" rx=\"2\" fill=\"#9aa7ad\"/><rect x=\"16\" y=\"17\" width=\"32\" height=\"25\" rx=\"9\" fill=\"#eef2f3\" stroke=\"#c5cfd3\" stroke-width=\"1\"/><g class=\"av-eyes\"><circle cx=\"26\" cy=\"29\" r=\"4\" fill=\"#1d1b26\"/><circle cx=\"38\" cy=\"29\" r=\"4\" fill=\"#1d1b26\"/><circle cx=\"27.4\" cy=\"27.6\" r=\"1.2\" fill=\"#fff\"/><circle cx=\"39.4\" cy=\"27.6\" r=\"1.2\" fill=\"#fff\"/></g><path d=\"M28 36.5L36 36.5\" stroke=\"#1d1b26\" stroke-width=\"1.6\" stroke-linecap=\"round\"/></svg>"}};
var ORDER=['rec','fr','kid','bot'];
var st={l:'rec',q:0},tok=0,timers=[];
var reduce=window.matchMedia&&window.matchMedia('(prefers-reduced-motion: reduce)').matches;
var ask=R.querySelector('.abt-ask'),ans=R.querySelector('.abt-ans'),txt=R.querySelector('.abt-txt'),re=R.querySelector('.abt-re'),rb=R.querySelector('.abt-rb'),qm=R.querySelector('.abt-qm');
var las=R.querySelectorAll('.abt-la');
function esc(s){return s.replace(/&/g,'&amp;').replace(/</g,'&lt;');}
function words(s){return esc(s).replace(/\S+/g,function(m){return '<span class="abt-w">'+m+'</span>';});}
function seg(s){var o='';s.replace(/\{([^}]*)\}|([^{]+)/g,function(m,u,p){if(u!==undefined){o+='<span class="abt-u">'+words(u)+'</span>';}else{o+=words(p);}return m;});return o;}
function count(s){var m=s.match(/\{[^}]*\}/g);return m?m.length:0;}
function render(s){
if(s.indexOf('|')<0)return seg(s);
return s.split('|').map(function(line){
var lab='',rest=line,m=line.match(/^([A-Z][A-Za-z ]{1,12}\d?):\s/);
if(m){lab='<span class="abt-lab">'+m[1]+'</span>';rest=line.slice(m[0].length);}
var end=/^(Please|End of)/.test(line)?' abt-end':'';
return '<span class="abt-line'+end+'">'+lab+seg(rest)+'</span>';
}).join('');
}
function clear(){timers.forEach(clearTimeout);timers=[];}
function later(f,ms){timers.push(setTimeout(f,ms));}
var MAX=0;
ORDER.forEach(function(l){D.ans[l].forEach(function(a){MAX=Math.max(MAX,count(a));});});
function meter(){
R.querySelectorAll('.abt-mr').forEach(function(r){
var l=r.getAttribute('data-l'),n=count(D.ans[l][st.q]);
r.querySelector('.abt-mb').style.width=(n/MAX*100)+'%';
r.querySelector('.abt-mv').textContent=n;
r.classList.toggle('abt-cur',l===st.l);
});
}
function show(){
clear();
var t=++tok,l=st.l,q=st.q;
R.setAttribute('data-l',l);
las.forEach(function(a){a.innerHTML=D.av[l];});
ask.textContent=D.ask[l][q];
rb.textContent=D.react[l][q];
re.classList.remove('abt-on');
txt.classList.remove('abt-show');
txt.innerHTML=render(D.ans[l][q]);
var ws=txt.querySelectorAll('.abt-w');
meter();
if(reduce){ans.classList.remove('abt-typing');txt.classList.add('abt-show');re.classList.add('abt-on');return;}
ans.classList.add('abt-typing');
var step=l==='bot'?42:30;
ws.forEach(function(w,i){w.style.transitionDelay=(i*step)+'ms';});
later(function(){if(t!==tok)return;ans.classList.remove('abt-typing');void txt.offsetWidth;txt.classList.add('abt-show');},650);
later(function(){if(t!==tok)return;re.classList.add('abt-on');},650+ws.length*step+450);
}
function press(sel,el){R.querySelectorAll(sel).forEach(function(b){b.setAttribute('aria-pressed',b===el?'true':'false');});}
R.querySelectorAll('.abt-l').forEach(function(b){b.addEventListener('click',function(){
if(st.l===b.getAttribute('data-l'))return;
st.l=b.getAttribute('data-l');press('.abt-l',b);
qm.classList.remove('abt-pop');void qm.offsetWidth;qm.classList.add('abt-pop');
show();
});});
R.querySelectorAll('.abt-q').forEach(function(b){b.addEventListener('click',function(){
var q=+b.getAttribute('data-q');
if(st.q===q)return;
st.q=q;press('.abt-q',b);show();
});});
var hl=R.querySelector('.abt-hl');
hl.addEventListener('click',function(){
var on=hl.getAttribute('aria-pressed')!=='true';
hl.setAttribute('aria-pressed',on?'true':'false');
hl.textContent=on?'Hide highlights':'Highlight them';
R.classList.toggle('abt-hlon',on);
});
show();
})();
</script>
