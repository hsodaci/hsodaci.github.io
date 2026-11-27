---
layout: default
---
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Figtree:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<style>
.adt{--rec:#3b6fe0;--rec-s:#dce6fb;--fr:#e8603f;--fr-s:#fbe0d8;--kid:#e8a514;--kid-s:#fbedc8;--bot:#13a184;--bot-s:#d3f0e8;--bg:#f5f2ec;--ink:#1d1b26;--mut:#5f5d6b;display:flex;flex-direction:column;align-items:center;gap:12px;max-width:430px;margin:-3.5rem auto 3rem;padding:20px 22px 18px;border-radius:20px;background:var(--bg);color:var(--ink)!important;text-decoration:none!important;text-align:center;transition:transform .25s,box-shadow .25s}
body[data-theme="dark"] .adt{--rec:#7aa2ff;--rec-s:#2b3a5e;--fr:#ff8f72;--fr-s:#55332d;--kid:#ffc857;--kid-s:#524425;--bot:#3fd3b1;--bot-s:#1f4a42;--bg:#24232c;--ink:#efece6;--mut:#b3b0bc}
.adt:hover{transform:translateY(-3px);box-shadow:0 14px 30px -18px rgba(0,0,0,.5)}
.adt-avs{display:flex}
.adt .av{width:44px;height:44px;border-radius:50%;border:3px solid var(--bg);margin-left:-9px;transition:transform .25s}
.adt .av:first-child{margin-left:0}
.adt:hover .av{transform:translateY(-4px)}
.adt:hover .av:nth-child(2){transition-delay:.05s}
.adt:hover .av:nth-child(3){transition-delay:.1s}
.adt:hover .av:nth-child(4){transition-delay:.15s}
.adt-tx{font-size:15px;line-height:1.55;color:var(--mut)}
.adt-tx b{color:var(--ink)!important;font-weight:700}
.adt-go{font-size:14.5px;font-weight:700;color:var(--ink);border-bottom:2px solid var(--ink);padding-bottom:1px}
.adt .av-eyes{transform-origin:center;transform-box:fill-box;animation:adtblink 4.5s infinite}
@keyframes adtblink{0%,92%,100%{transform:scaleY(1)}95%{transform:scaleY(.12)}}
@media (max-width:600px){.adt{margin:-1rem 16px 2.5rem}}
.adt{font-family:"Figtree",system-ui,-apple-system,"Segoe UI",sans-serif}
.wrapper .author{font-family:"Figtree",system-ui,-apple-system,"Segoe UI",sans-serif;--hi:#1d1b26;--hm:#5f5d6b;--hl:rgba(29,27,38,.14);--hacc:#3b6fe0}
body[data-theme="dark"] .wrapper .author{--hi:#efece6;--hm:#b3b0bc;--hl:rgba(255,255,255,.16);--hacc:#8aaeff}
.wrapper .author .author-avatar{width:96px;height:96px;box-shadow:0 0 0 4px var(--hl)}
.wrapper .author h2.author-name{font-family:inherit;font-size:clamp(34px,6vw,46px);font-weight:800;letter-spacing:-.03em;line-height:1.05;margin:18px 0 12px;color:var(--hi)}
.wrapper .author p.author-bio{font-size:17px;line-height:1.65;max-width:470px;color:var(--hm);opacity:1}
.wrapper .author .author-links{margin-top:20px;display:flex;justify-content:center;flex-wrap:wrap;gap:8px}
.wrapper .author .author-links a,body[data-theme="dark"] .wrapper .author .author-links a{font-family:inherit;font-size:14.5px;font-weight:700;color:var(--hi)!important;background:transparent!important;border:2px solid var(--hl)!important;border-radius:999px;padding:6px 16px;margin:0;opacity:1;text-decoration:none!important;transition:transform .2s,border-color .2s}
.wrapper .author .author-links a:hover,body[data-theme="dark"] .wrapper .author .author-links a:hover{border-color:var(--hi)!important;transform:translateY(-2px)}
</style>
<div class="adt-w"><a class="adt" href="/about/"><span class="adt-avs"><svg class="av av-t" viewBox="0 0 64 64" aria-hidden="true"><circle cx="32" cy="32" r="32" style="fill:var(--rec-s)"/><path d="M10 64C10 51 20 44 32 44C44 44 54 51 54 64Z" style="fill:var(--rec)"/><path d="M26 44.5L32 53L38 44.5Z" fill="#fff"/><path d="M30.6 47.5L33.4 47.5L34.4 58L32 61L29.6 58Z" fill="#1d1b26"/><rect x="29" y="35" width="6" height="10" fill="#e8b48f"/><circle cx="32" cy="27" r="11" fill="#e8b48f"/><path d="M21 26C20 16 27 12.5 33 13C40 13.5 44 18 43 25C40 20 34 19 28 21C25 22 23 24 21 26Z" fill="#2b2333"/><g fill="none" stroke="#1d1b26" stroke-width="1.4"><circle cx="27.6" cy="28" r="3.2"/><circle cx="36.4" cy="28" r="3.2"/><path d="M30.8 28L33.2 28"/></g><path d="M29.5 33.2Q32 34.4 34.5 33.2" fill="none" stroke="#1d1b26" stroke-width="1.3" stroke-linecap="round"/></svg><svg class="av av-t" viewBox="0 0 64 64" aria-hidden="true"><circle cx="32" cy="32" r="32" style="fill:var(--fr-s)"/><path d="M19 30C18 16 25 12 32 12C40 12 46 17 45 30L46 46L18 46Z" fill="#6b3a28"/><path d="M10 64C10 51 20 44 32 44C44 44 54 51 54 64Z" style="fill:var(--fr)"/><rect x="29" y="35" width="6" height="10" fill="#f3cfae"/><circle cx="32" cy="27" r="11" fill="#f3cfae"/><path d="M21 26C22 16 30 13 36 15C41 17 43 21 43 26C37 23 31 21 27.5 18C25.5 21 23.5 23.5 21 26Z" fill="#6b3a28"/><circle cx="28" cy="27.8" r="1.3" fill="#1d1b26"/><circle cx="36" cy="27.8" r="1.3" fill="#1d1b26"/><path d="M28 31.6Q32 35.6 36 31.6" fill="none" stroke="#1d1b26" stroke-width="1.5" stroke-linecap="round"/></svg><svg class="av av-t" viewBox="0 0 64 64" aria-hidden="true"><circle cx="32" cy="32" r="32" style="fill:var(--kid-s)"/><circle cx="17" cy="27" r="6" fill="#2b2333"/><circle cx="47" cy="27" r="6" fill="#2b2333"/><path d="M16 64C16 54 23 49 32 49C41 49 48 54 48 64Z" style="fill:var(--kid)"/><rect x="29" y="40" width="6" height="10" fill="#c98d66"/><circle cx="32" cy="30" r="13" fill="#c98d66"/><path d="M19 29C19 19 26 15.5 32 15.5C39 15.5 45 19.5 45 29C40 24.5 35.5 22.5 32 22.5C28 22.5 23.5 24.5 19 29Z" fill="#2b2333"/><circle cx="27" cy="30.5" r="1.7" fill="#1d1b26"/><circle cx="37" cy="30.5" r="1.7" fill="#1d1b26"/><circle cx="24" cy="35" r="2.2" fill="#ff8f7d" opacity=".55"/><circle cx="40" cy="35" r="2.2" fill="#ff8f7d" opacity=".55"/><path d="M27.5 35Q32 40 36.5 35Z" fill="#1d1b26"/></svg><svg class="av av-t" viewBox="0 0 64 64" aria-hidden="true"><circle cx="32" cy="32" r="32" style="fill:var(--bot-s)"/><rect x="17" y="48" width="30" height="20" rx="7" style="fill:var(--bot)"/><rect x="29" y="41" width="6" height="8" fill="#9aa7ad"/><path d="M32 18L32 11" stroke="#9aa7ad" stroke-width="2"/><circle cx="32" cy="9.5" r="3.2" style="fill:var(--bot)"/><rect x="12.5" y="25" width="4.5" height="10" rx="2" fill="#9aa7ad"/><rect x="47" y="25" width="4.5" height="10" rx="2" fill="#9aa7ad"/><rect x="16" y="17" width="32" height="25" rx="9" fill="#eef2f3" stroke="#c5cfd3" stroke-width="1"/><g class="av-eyes"><circle cx="26" cy="29" r="4" fill="#1d1b26"/><circle cx="38" cy="29" r="4" fill="#1d1b26"/><circle cx="27.4" cy="27.6" r="1.2" fill="#fff"/><circle cx="39.4" cy="27.6" r="1.2" fill="#fff"/></g><path d="M28 36.5L36 36.5" stroke="#1d1b26" stroke-width="1.6" stroke-linecap="round"/></svg></span><span class="adt-tx">How would you describe your job to a recruiter, a friend, a five-year-old, and a robot? Probably four different ways. That is called <b>audience design</b>, and it is what I study.</span><span class="adt-go">See how I’d answer <span aria-hidden="true">→</span></span></a>
