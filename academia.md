---
title: Academia
permalink: /academia/
layout: page
excerpt: Publications on human–robot interaction, speech adaptation, and robot-assisted language learning.
comments: false
---
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Figtree:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<style>
.header:has(+ .page-content .aca){display:none}
.aca{--ink:#1d1b26;--muted:#6a6878;--card:#f5f2ec;--card2:#ebe6dd;--me:#ffffff;--line:rgba(29,27,38,.12);--rec:#3b6fe0;--rec-s:#dce6fb;--fr:#e8603f;--fr-s:#fbe0d8;--kid:#e8a514;--kid-s:#fbedc8;--bot:#13a184;--bot-s:#d3f0e8;--gold-s:#fbedc8;--gold:#8a5a00;--c:var(--rec);--cs:var(--rec-s)}
body[data-theme="dark"] .aca{--ink:#efece6;--muted:#a6a3b0;--card:#24232c;--card2:#2e2d38;--me:#33323e;--line:rgba(255,255,255,.12);--rec:#7aa2ff;--rec-s:#2b3a5e;--fr:#ff8f72;--fr-s:#55332d;--kid:#ffc857;--kid-s:#524425;--bot:#3fd3b1;--bot-s:#1f4a42;--gold-s:#4a3d1c;--gold:#ffd27a}
.aca[data-v="fr"]{--c:var(--fr);--cs:var(--fr-s)}
.aca[data-v="kid"]{--c:var(--kid);--cs:var(--kid-s)}
.aca[data-v="bot"]{--c:var(--bot);--cs:var(--bot-s)}
.aca{font-family:"Figtree",system-ui,-apple-system,"Segoe UI",sans-serif;color:var(--ink);font-size:16.5px;line-height:1.55;padding:6px 0 30px}
.aca *{box-sizing:border-box}
.aca p{margin:0}
.aca button{font-family:inherit;cursor:pointer}
.aca .av{display:block;border-radius:50%}
.aca p.aca-kick{font-size:13px;font-weight:700;letter-spacing:.14em;text-transform:uppercase;color:var(--muted);margin-bottom:6px}
.aca h1.aca-h1{font-family:inherit;font-size:clamp(44px,9vw,72px);font-weight:800;line-height:1;letter-spacing:-.03em;margin:0 0 16px;color:var(--ink)}
.aca h1.aca-h1::after{content:".";color:var(--c);transition:color .35s}
.aca p.aca-lead{font-size:19px;max-width:560px;margin-bottom:22px}
.aca-sw{position:sticky;top:8px;z-index:5;display:grid;grid-template-columns:repeat(4,1fr);gap:6px;padding:6px;border-radius:999px;background:var(--card);box-shadow:0 8px 20px -16px rgba(0,0,0,.5)}
.aca .aca-s{display:flex;align-items:center;justify-content:center;gap:8px;border:0;border-radius:999px;background:transparent;color:var(--ink);font-size:15px;font-weight:600;padding:6px 10px 6px 6px;transition:background .2s,color .2s}
.aca .aca-s .av-s{width:30px;height:30px;flex:0 0 30px}
.aca .aca-s:hover{background:var(--card2)}
.aca .aca-s[aria-pressed="true"]{background:var(--ink);color:var(--card)}
.aca .aca-s:focus-visible,.aca .aca-btn:focus-visible{outline:3px solid var(--c);outline-offset:2px}
.aca p.aca-why{font-size:14px;color:var(--muted);margin:10px 0 0 6px}
.aca p.aca-why a{color:var(--ink)!important;font-weight:700;text-decoration:none!important;background:linear-gradient(transparent 60%,var(--cs) 60%);transition:background .35s}
.aca-list{display:flex;flex-direction:column;gap:22px;margin-top:30px}
.aca-card{display:grid;grid-template-columns:96px 1fr;gap:18px;background:var(--card);border-radius:22px;padding:24px 24px 22px}
.aca-side{display:flex;flex-direction:column;gap:4px}
.aca .aca-year{font-size:36px;font-weight:800;letter-spacing:-.03em;line-height:1}
.aca .aca-kind{font-size:12.5px;font-weight:700;letter-spacing:.06em;text-transform:uppercase;color:var(--muted);line-height:1.3}
.aca-main{min-width:0}
.aca p.aca-award{display:inline-flex;align-items:center;gap:7px;background:var(--gold-s);color:var(--gold);font-size:13.5px;font-weight:700;padding:4px 12px 4px 6px;border-radius:999px;margin-bottom:10px}
.aca .aca-rib{width:22px;height:22px;flex:0 0 22px}
.aca h2.aca-t{font-family:inherit;font-size:21px;font-weight:700;line-height:1.3;letter-spacing:-.01em;margin:0 0 8px;color:var(--ink)}
.aca p.aca-au{font-size:15px;line-height:1.5;margin-bottom:4px}
.aca p.aca-au strong{color:var(--ink)!important;font-weight:800;background:linear-gradient(transparent 62%,var(--cs) 62%);transition:background .35s}
.aca p.aca-meta{font-size:13.5px;color:var(--muted);line-height:1.45}
.aca-read{margin-top:16px;background:var(--me);border-radius:16px;padding:14px 16px 16px;border-left:5px solid var(--c);transition:border-color .35s}
.aca-vh{display:flex;flex-wrap:wrap;align-items:center;justify-content:space-between;gap:10px;margin-bottom:8px}
.aca .aca-who{font-size:13px;font-weight:700;letter-spacing:.06em;text-transform:uppercase;color:var(--c);transition:color .35s}
.aca .aca-wc{font-size:12.5px;font-weight:700;color:var(--muted);background:var(--card2);border-radius:999px;padding:2px 9px;white-space:nowrap;font-variant-numeric:tabular-nums}
.aca .aca-v{display:none;font-size:15.5px;line-height:1.6}
.aca[data-v="res"] .aca-v[data-v="res"],.aca[data-v="fr"] .aca-v[data-v="fr"],.aca[data-v="kid"] .aca-v[data-v="kid"],.aca[data-v="bot"] .aca-v[data-v="bot"]{display:block;animation:acain .35s}
@keyframes acain{from{opacity:0;transform:translateY(4px)}}
.aca p.aca-v.aca-big{font-size:21px;font-weight:700;line-height:1.4}
.aca .aca-bl{display:block;font-size:15px}
.aca .aca-bl+.aca-bl{margin-top:4px}
.aca .aca-lab{display:inline-block;min-width:74px;font-size:11.5px;font-weight:700;letter-spacing:.08em;text-transform:uppercase;background:var(--bot);color:#fff;border-radius:5px;padding:1px 6px;margin-right:8px;vertical-align:1px;text-align:center}
body[data-theme="dark"] .aca .aca-lab{color:#17161d}
.aca .aca-bl.aca-end{color:var(--muted);font-weight:600;margin-top:8px}
.aca-tags{display:flex;flex-wrap:wrap;gap:6px;margin-top:14px}
.aca .aca-tag{font-size:12.5px;font-weight:600;color:var(--muted);border:1.5px solid var(--line);border-radius:999px;padding:2px 10px}
.aca-act{display:flex;flex-wrap:wrap;gap:8px;margin-top:16px}
.aca .aca-btn{display:inline-flex;align-items:center;gap:6px;font-size:14.5px;font-weight:700;border-radius:999px;padding:7px 15px;text-decoration:none!important;border:2px solid var(--line);background:transparent;color:var(--ink)!important;transition:transform .2s,border-color .2s,background .2s}
.aca .aca-btn:hover{transform:translateY(-2px);border-color:var(--ink)}
.aca .aca-btn.aca-pri{background:var(--ink);border-color:var(--ink);color:var(--card)!important}
.aca .aca-copy.aca-done{border-color:var(--bot);background:var(--bot-s)}
.aca[data-v="bot"] .aca-copy{border-color:var(--bot);box-shadow:0 0 0 4px var(--bot-s)}
.aca p.aca-out{display:flex;flex-wrap:wrap;gap:10px;justify-content:center;margin-top:34px}
.aca p.aca-out a{display:inline-flex;align-items:center;gap:6px;font-weight:700;font-size:15px;text-decoration:none!important;border-radius:999px;padding:8px 16px;border:2px solid var(--line);color:var(--ink)!important;transition:transform .2s,border-color .2s}
.aca p.aca-out a:hover{transform:translateY(-2px);border-color:var(--ink)}
.aca .av-eyes{transform-origin:center;transform-box:fill-box;animation:acablink 4.5s infinite}
@keyframes acablink{0%,92%,100%{transform:scaleY(1)}95%{transform:scaleY(.12)}}
@media (max-width:600px){
.aca-sw{border-radius:18px;gap:4px;padding:5px}
.aca .aca-s{flex-direction:column;gap:3px;padding:6px 2px;border-radius:14px;font-size:12.5px}
.aca .aca-s .av-s{width:28px;height:28px}
.aca-card{grid-template-columns:1fr;gap:10px;padding:18px 16px}
.aca-side{flex-direction:row;align-items:baseline;gap:10px}
.aca .aca-year{font-size:28px}
.aca h2.aca-t{font-size:19px}
.aca-read{padding:12px 13px 14px}
.aca .aca-lab{min-width:64px}
}
@media (prefers-reduced-motion:reduce){.aca *{animation:none!important;transition:none!important}}
</style>
<div class="aca" data-v="res">
<p class="aca-kick">Academia</p>
<h1 class="aca-h1">Papers</h1>
<p class="aca-lead">Peer-reviewed work on how people talk to robots, and how children learn from them. Each paper can be read four ways. Pick your reader.</p>
<div class="aca-sw" role="group" aria-label="Read the papers as"><button type="button" class="aca-s" data-v="res" aria-pressed="true"><svg class="av av-s" viewBox="0 0 64 64" aria-hidden="true"><circle cx="32" cy="32" r="32" style="fill:var(--rec-s)"/><path d="M10 64C10 51 20 44 32 44C44 44 54 51 54 64Z" style="fill:var(--rec)"/><path d="M26 44.5L32 53L38 44.5Z" fill="#fff"/><path d="M30.6 47.5L33.4 47.5L34.4 58L32 61L29.6 58Z" fill="#1d1b26"/><rect x="29" y="35" width="6" height="10" fill="#e8b48f"/><circle cx="32" cy="27" r="11" fill="#e8b48f"/><path d="M21 26C20 16 27 12.5 33 13C40 13.5 44 18 43 25C40 20 34 19 28 21C25 22 23 24 21 26Z" fill="#2b2333"/><g fill="none" stroke="#1d1b26" stroke-width="1.4"><circle cx="27.6" cy="28" r="3.2"/><circle cx="36.4" cy="28" r="3.2"/><path d="M30.8 28L33.2 28"/></g><path d="M29.5 33.2Q32 34.4 34.5 33.2" fill="none" stroke="#1d1b26" stroke-width="1.3" stroke-linecap="round"/></svg><span>Researcher</span></button><button type="button" class="aca-s" data-v="fr" aria-pressed="false"><svg class="av av-s" viewBox="0 0 64 64" aria-hidden="true"><circle cx="32" cy="32" r="32" style="fill:var(--fr-s)"/><path d="M19 30C18 16 25 12 32 12C40 12 46 17 45 30L46 46L18 46Z" fill="#6b3a28"/><path d="M10 64C10 51 20 44 32 44C44 44 54 51 54 64Z" style="fill:var(--fr)"/><rect x="29" y="35" width="6" height="10" fill="#f3cfae"/><circle cx="32" cy="27" r="11" fill="#f3cfae"/><path d="M21 26C22 16 30 13 36 15C41 17 43 21 43 26C37 23 31 21 27.5 18C25.5 21 23.5 23.5 21 26Z" fill="#6b3a28"/><circle cx="28" cy="27.8" r="1.3" fill="#1d1b26"/><circle cx="36" cy="27.8" r="1.3" fill="#1d1b26"/><path d="M28 31.6Q32 35.6 36 31.6" fill="none" stroke="#1d1b26" stroke-width="1.5" stroke-linecap="round"/></svg><span>Friend</span></button><button type="button" class="aca-s" data-v="kid" aria-pressed="false"><svg class="av av-s" viewBox="0 0 64 64" aria-hidden="true"><circle cx="32" cy="32" r="32" style="fill:var(--kid-s)"/><circle cx="17" cy="27" r="6" fill="#2b2333"/><circle cx="47" cy="27" r="6" fill="#2b2333"/><path d="M16 64C16 54 23 49 32 49C41 49 48 54 48 64Z" style="fill:var(--kid)"/><rect x="29" y="40" width="6" height="10" fill="#c98d66"/><circle cx="32" cy="30" r="13" fill="#c98d66"/><path d="M19 29C19 19 26 15.5 32 15.5C39 15.5 45 19.5 45 29C40 24.5 35.5 22.5 32 22.5C28 22.5 23.5 24.5 19 29Z" fill="#2b2333"/><circle cx="27" cy="30.5" r="1.7" fill="#1d1b26"/><circle cx="37" cy="30.5" r="1.7" fill="#1d1b26"/><circle cx="24" cy="35" r="2.2" fill="#ff8f7d" opacity=".55"/><circle cx="40" cy="35" r="2.2" fill="#ff8f7d" opacity=".55"/><path d="M27.5 35Q32 40 36.5 35Z" fill="#1d1b26"/></svg><span>5-year-old</span></button><button type="button" class="aca-s" data-v="bot" aria-pressed="false"><svg class="av av-s" viewBox="0 0 64 64" aria-hidden="true"><circle cx="32" cy="32" r="32" style="fill:var(--bot-s)"/><rect x="17" y="48" width="30" height="20" rx="7" style="fill:var(--bot)"/><rect x="29" y="41" width="6" height="8" fill="#9aa7ad"/><path d="M32 18L32 11" stroke="#9aa7ad" stroke-width="2"/><circle cx="32" cy="9.5" r="3.2" style="fill:var(--bot)"/><rect x="12.5" y="25" width="4.5" height="10" rx="2" fill="#9aa7ad"/><rect x="47" y="25" width="4.5" height="10" rx="2" fill="#9aa7ad"/><rect x="16" y="17" width="32" height="25" rx="9" fill="#eef2f3" stroke="#c5cfd3" stroke-width="1"/><g class="av-eyes"><circle cx="26" cy="29" r="4" fill="#1d1b26"/><circle cx="38" cy="29" r="4" fill="#1d1b26"/><circle cx="27.4" cy="27.6" r="1.2" fill="#fff"/><circle cx="39.4" cy="27.6" r="1.2" fill="#fff"/></g><path d="M28 36.5L36 36.5" stroke="#1d1b26" stroke-width="1.6" stroke-linecap="round"/></svg><span>Robot</span></button></div>
<p class="aca-why">Why four versions? That is <a href="/about/">audience design</a>.</p>
<div class="aca-list">
<article class="aca-card">
<div class="aca-side"><span class="aca-year">2026</span><span class="aca-kind">Conference paper</span></div>
<div class="aca-main">
<p class="aca-award"><svg class="aca-rib" viewBox="0 0 24 24" aria-hidden="true"><path d="M7 13L4.5 21L8.5 19.5L11 22.5L12.5 14Z" fill="#c6532f"/><path d="M17 13L19.5 21L15.5 19.5L13 22.5L11.5 14Z" fill="#e8603f"/><circle cx="12" cy="9" r="7" fill="#f2b33d"/><circle cx="12" cy="9" r="4.4" fill="none" stroke="#fff" stroke-width="1.4"/></svg>Honorable Mention Award · HRI 2026</p><h2 class="aca-t">Real-Time Speech Adaptation to Human and Robot Audiences</h2>
<p class="aca-au"><strong>Sodacı, H.</strong>, &amp; Küntay, A. C.</p>
<p class="aca-meta">Companion Proceedings of the 21st ACM/IEEE International Conference on Human-Robot Interaction (HRI Companion ’26) · 392–396 · 2026</p>
<div class="aca-read">
<div class="aca-vh"><span class="aca-who"></span><span class="aca-wc"></span></div>
<p class="aca-v" data-v="res">Audience design (adapting communication to an audience&#39;s needs and shared knowledge) poses unique challenges in human-robot interaction (HRI), where speakers lack prior experience with robots and must rely on real-time communicative cues. In a word-guessing game, participants described words to either a robot or a human audience, who guessed the words with a 25% error rate. Descriptions were coded for the number of semantic details (distinct meaning-relevant units). Participants produced more semantic details for robots than humans, with a marginal trend suggesting speakers reduced details for humans but maintained elaboration for robots during consistent success. This asymmetry hints at persistent assumptions about robot competence that behavioral success may not override.</p>
<p class="aca-v" data-v="fr">Do people talk to robots differently than to other people? In a word-guessing game, people described words to either a robot or a human partner. Both partners guessed wrong one time in four. People packed more meaningful details into their descriptions for the robot. When the game was going well, they seemed to trim details for the human but kept explaining just as much to the robot, as if success alone did not convince them the robot understood.</p>
<p class="aca-v aca-big" data-v="kid">People gave a robot more clues than a person in a word-guessing game.</p>
<div class="aca-v" data-v="bot"><span class="aca-bl"><span class="aca-lab">Type</span>conference paper</span><span class="aca-bl"><span class="aca-lab">Authors</span>Sodacı, H.; Küntay, A. C.</span><span class="aca-bl"><span class="aca-lab">Year</span>2026</span><span class="aca-bl"><span class="aca-lab">Venue</span>HRI Companion ’26</span><span class="aca-bl"><span class="aca-lab">Pages</span>392–396</span><span class="aca-bl"><span class="aca-lab">DOI</span>10.1145/3776734.3794422</span><span class="aca-bl aca-end">Citation ready. Copy?</span></div>
</div>
<div class="aca-tags"><span class="aca-tag">Social robots</span><span class="aca-tag">Audience design</span><span class="aca-tag">Speech adaptation</span><span class="aca-tag">Task-based interaction</span></div>
<div class="aca-act"><a class="aca-btn aca-pri" href="https://doi.org/10.1145/3776734.3794422" target="_blank" rel="noopener">Read the paper <span aria-hidden="true">↗</span></a><button type="button" class="aca-btn aca-copy" data-apa="Sodacı, H., &amp; Küntay, A. C. (2026). Real-time speech adaptation to human and robot audiences. Companion Proceedings of the 21st ACM/IEEE International Conference on Human-Robot Interaction, HRI Companion &#39;26, 392-396. https://doi.org/10.1145/3776734.3794422">Copy citation (APA)</button><a class="aca-btn aca-ln" href="/projects/talking-to-robots/">Project page: Talking to Robots <span aria-hidden="true">→</span></a></div>
</div>
</article>
<article class="aca-card">
<div class="aca-side"><span class="aca-year">2020</span><span class="aca-kind">Journal article</span></div>
<div class="aca-main">
<h2 class="aca-t">Teaching Turkish–Dutch kindergartners Dutch vocabulary with a social robot: Does the robot’s use of Turkish translations benefit children’s Dutch vocabulary learning?</h2>
<p class="aca-au">Leeuwestein, H., Barking, M., <strong>Sodacı, H.</strong>, Oudgenoeg-Paz, O., Verhagen, J., Vogt, P., Aarts, R., Spit, S., de Haas, M., de Wit, J., &amp; Leseman, P.</p>
<p class="aca-meta">Journal of Computer Assisted Learning, 37(3) · 603–620 · 2020</p>
<div class="aca-read">
<div class="aca-vh"><span class="aca-who"></span><span class="aca-wc"></span></div>
<p class="aca-v" data-v="res">Providing first language (L1) translations in L2 vocabulary interventions may be beneficial for L2 vocabulary learning. However, in linguistically diverse L2 classrooms, teachers cannot provide L1 translations to all children. Social robots do offer such opportunities, as they can be programmed to speak any combination of languages. This study investigates whether providing L1 translations in a robot-assisted L2 vocabulary training facilitates children&#39;s learning. Participants were Turkish-Dutch kindergartners (n = 67) who were taught six Dutch (L2) words for which they knew the L1 (Turkish), but not the L2 Dutch form. Half of these words were taught by a Turkish-Dutch bilingual robot, alongside their Turkish translations; the other half by a monolingual Dutch robot. Results indicated better performance in the Dutch-only condition than in the Turkish-Dutch condition. The majority of children preferred working with the bilingual robot, but children&#39;s preference did not affect word learning. Contrary to the prediction, the study found no evidence for a facilitating effect of providing L1 translations through a robot on bilingual children&#39;s L2 word learning.</p>
<p class="aca-v" data-v="fr">Can a robot that speaks children’s home language help them learn a new one? 67 Turkish–Dutch kindergartners learned six Dutch words from a robot. For half of the words, the robot also gave the Turkish translation. For the other half, it spoke only Dutch. Most children preferred the bilingual robot, but they did better on the words taught in Dutch only. How much they liked the robot did not change how much they learned.</p>
<p class="aca-v aca-big" data-v="kid">Kids liked the robot that spoke Turkish best, but they learned more Dutch words from the robot that spoke only Dutch.</p>
<div class="aca-v" data-v="bot"><span class="aca-bl"><span class="aca-lab">Type</span>journal article</span><span class="aca-bl"><span class="aca-lab">Authors</span>Leeuwestein, H.; Barking, M.; Sodacı, H.; and 8 others</span><span class="aca-bl"><span class="aca-lab">Year</span>2020</span><span class="aca-bl"><span class="aca-lab">Journal</span>Journal of Computer Assisted Learning</span><span class="aca-bl"><span class="aca-lab">Volume</span>37(3)</span><span class="aca-bl"><span class="aca-lab">Pages</span>603–620</span><span class="aca-bl"><span class="aca-lab">DOI</span>10.1111/jcal.12510</span><span class="aca-bl aca-end">Citation ready. Copy?</span></div>
</div>
<div class="aca-tags"><span class="aca-tag">First language translations</span><span class="aca-tag">Kindergartners</span><span class="aca-tag">Robot-assisted language learning</span><span class="aca-tag">Second language</span><span class="aca-tag">Vocabulary</span></div>
<div class="aca-act"><a class="aca-btn aca-pri" href="https://doi.org/10.1111/jcal.12510" target="_blank" rel="noopener">Read the paper <span aria-hidden="true">↗</span></a><button type="button" class="aca-btn aca-copy" data-apa="Leeuwestein, H., Barking, M., Sodacı, H., Oudgenoeg-Paz, O., Verhagen, J., Vogt, P., Aarts, R., Spit, S., de Haas, M., de Wit, J., &amp; Leseman, P. (2020). Teaching Turkish-Dutch kindergartners Dutch vocabulary with a social robot: Does the robot&#39;s use of Turkish translations benefit children&#39;s Dutch vocabulary learning? Journal of Computer Assisted Learning, 37(3), 603-620. https://doi.org/10.1111/jcal.12510">Copy citation (APA)</button><a class="aca-btn aca-ln" href="/projects/robots-as-tutors/">Project page: Robots as Tutors <span aria-hidden="true">→</span></a></div>
</div>
</article>
</div>
<p class="aca-out"><a href="https://orcid.org/{{ site.author.orcid }}" target="_blank" rel="noopener">ORCID <span aria-hidden="true">↗</span></a><a href="/assets/HS_resume_202611.pdf" target="_blank" rel="noopener">Resume <span aria-hidden="true">↗</span></a></p>
</div>
<script>
(function(){
var R=document.querySelector('.aca');
if(!R)return;
var NAMES={res:'Read as a researcher · abstract',fr:'Read as a friend · plain words',kid:'Read as a 5-year-old · one line',bot:'Read as a robot · metadata'};
function wc(el){var t=(el.textContent||'').trim();return t?t.split(/\s+/).length:0;}
function set(v){
R.setAttribute('data-v',v);
R.querySelectorAll('.aca-s').forEach(function(b){b.setAttribute('aria-pressed',b.getAttribute('data-v')===v?'true':'false');});
R.querySelectorAll('.aca-card').forEach(function(c){
var p=c.querySelector('.aca-v[data-v="'+v+'"]');
c.querySelector('.aca-who').textContent=NAMES[v];
c.querySelector('.aca-wc').textContent=v==='bot'?'machine-readable':wc(p)+' words';
});
}
R.querySelectorAll('.aca-s').forEach(function(b){b.addEventListener('click',function(){set(b.getAttribute('data-v'));});});
R.querySelectorAll('.aca-copy').forEach(function(b){b.addEventListener('click',function(){
var t=b.getAttribute('data-apa'),lab=b.textContent;
function ok(){b.textContent='Copied ✓';b.classList.add('aca-done');setTimeout(function(){b.textContent=lab;b.classList.remove('aca-done');},1800);}
if(navigator.clipboard&&navigator.clipboard.writeText){navigator.clipboard.writeText(t).then(ok,function(){fallback(t);ok();});}else{fallback(t);ok();}
});});
function fallback(t){var a=document.createElement('textarea');a.value=t;a.style.position='fixed';a.style.opacity='0';document.body.appendChild(a);a.select();try{document.execCommand('copy');}catch(e){}document.body.removeChild(a);}
set('res');
})();
</script>
