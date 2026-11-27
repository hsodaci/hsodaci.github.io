---
title: Academia
permalink: /academia/
layout: page
excerpt: Publications on human–robot interaction, speech adaptation, and robot-assisted language learning.
comments: false
---
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Figtree:wght@400;500;600;700;800;900&display=swap" rel="stylesheet">
<style>
.header:has(+ .page-content .ac2){display:none}
.ac2{--desk:#dde4ec;--paper:#fffdf8;--paper2:#f3efe6;--ink:#1d1b26;--muted:#686676;--line:rgba(29,27,38,.16);--red:#d23f2a;--blue:#3b6fe0;--blue-s:#dce6fb;--note:#ffe07a;--noteink:#3a2f00;--sh:rgba(25,32,48,.42)}
body[data-theme="dark"] .ac2{--desk:#1e222b;--paper:#2b2a33;--paper2:#25242d;--ink:#efece6;--muted:#a9a6b3;--line:rgba(255,255,255,.16);--red:#ff6a52;--blue:#8aaeff;--blue-s:#2b3a5e;--note:#f2d469;--noteink:#2b2300;--sh:rgba(0,0,0,.7)}
.ac2{font-family:"Figtree",system-ui,-apple-system,"Segoe UI",sans-serif;color:var(--ink);padding:4px 0 30px}
.ac2 *{box-sizing:border-box}
.ac2 p{margin:0}
.ac2 button{font-family:inherit;cursor:pointer}
.ac2-mast{border-top:7px solid var(--ink);border-bottom:1.5px solid var(--ink);padding:10px 0 12px;margin-bottom:26px}
.ac2 h1.ac2-h1{font-family:inherit;font-size:clamp(52px,12vw,104px);font-weight:900;letter-spacing:-.045em;line-height:.92;margin:0;color:var(--ink)}
.ac2-desk{background:var(--desk);border-radius:26px;padding:46px 36px 54px;display:flex;flex-direction:column;gap:54px}
.ac2-page{position:relative;background:var(--paper);padding:46px 44px 22px;border-radius:3px;box-shadow:7px 8px 0 0 var(--paper2),7px 8px 0 1px var(--line),0 22px 44px -24px var(--sh);transition:transform .5s cubic-bezier(.3,.8,.3,1),box-shadow .5s}
.ac2-page::after{content:"";position:absolute;right:0;bottom:0;width:34px;height:34px;background:linear-gradient(315deg,var(--desk) 50%,var(--paper2) 50%);box-shadow:-3px -3px 6px -4px var(--sh)}
.ac2-p0{transform:rotate(-1deg)}
.ac2-p1{transform:rotate(.8deg);box-shadow:-7px 8px 0 0 var(--paper2),-7px 8px 0 1px var(--line),0 22px 44px -24px var(--sh)}
.ac2-page:hover{transform:rotate(0) translateY(-4px);box-shadow:7px 8px 0 0 var(--paper2),7px 8px 0 1px var(--line),0 30px 54px -26px var(--sh)}
.ac2 p.ac2-band{font-size:12.5px;font-weight:700;letter-spacing:.05em;text-transform:uppercase;color:var(--muted);line-height:1.5;padding:0 140px 10px 0;border-bottom:1.5px solid var(--ink)}
.ac2 h2.ac2-t{font-family:inherit;font-size:29px;font-weight:800;line-height:1.18;letter-spacing:-.02em;margin:24px 0 14px;color:var(--ink)}
.ac2-p0 h2.ac2-t{padding-right:220px}
.ac2 p.ac2-au{font-size:15.5px;line-height:1.55;color:var(--ink)}
.ac2 p.ac2-au strong{color:var(--ink)!important;font-weight:800;background:linear-gradient(transparent 62%,var(--blue-s) 62%)}
.ac2-absw{margin-top:22px;padding-top:16px;border-top:1px solid var(--line)}
.ac2 .ac2-lab{display:block;font-size:11.5px;font-weight:800;letter-spacing:.18em;text-transform:uppercase;color:var(--ink);margin-bottom:8px}
.ac2 p.ac2-abs{font-size:15px;line-height:1.66;column-count:2;column-gap:32px;column-rule:1px solid var(--line)}
.ac2 p.ac2-kw{margin-top:18px;font-size:14px;color:var(--muted);line-height:1.5}
.ac2 p.ac2-kw .ac2-lab{display:inline;margin:0 10px 0 0}
.ac2-foot{display:flex;justify-content:space-between;align-items:center;gap:12px;margin-top:26px;padding-top:10px;border-top:1px solid var(--line);font-size:13.5px}
.ac2 a.ac2-doi{color:var(--blue)!important;font-weight:700;text-decoration:none!important;overflow-wrap:anywhere}
.ac2 a.ac2-doi:hover{text-decoration:underline!important}
.ac2 .ac2-pn{font-weight:800;color:var(--muted);font-variant-numeric:tabular-nums;margin-right:30px}
.ac2-stamp{position:absolute;top:104px;right:34px;z-index:2;transform:rotate(-12deg);opacity:0}
.ac2-stamp span{display:block;border:3px solid var(--red);border-radius:10px;padding:8px 13px;box-shadow:inset 0 0 0 2px var(--paper),inset 0 0 0 4px var(--red);color:var(--red);font-size:13.5px;font-weight:900;letter-spacing:.12em;text-transform:uppercase;line-height:1.2;text-align:center}
.ac2-stamp.ac2-in{animation:ac2stamp .55s cubic-bezier(.2,1.4,.4,1) forwards}
@keyframes ac2stamp{0%{opacity:0;transform:rotate(-20deg) scale(2.2)}60%{opacity:.95;transform:rotate(-11deg) scale(.94)}100%{opacity:.9;transform:rotate(-12deg) scale(1)}}
.ac2-note{position:absolute;top:-18px;right:26px;z-index:3;width:118px;background:var(--note);color:var(--noteink);transform:rotate(3deg);box-shadow:0 10px 18px -10px rgba(0,0,0,.45);transition:width .35s cubic-bezier(.3,.8,.3,1),transform .35s}
.ac2-note::before{content:"";position:absolute;top:-9px;left:50%;width:54px;height:18px;margin-left:-27px;background:rgba(255,255,255,.55);transform:rotate(-4deg)}
body[data-theme="dark"] .ac2-note::before{background:rgba(255,255,255,.28)}
.ac2-note.ac2-open{width:min(340px,calc(100vw - 70px));transform:rotate(1deg)}
.ac2 .ac2-nb{display:block;width:100%;border:0;background:transparent;color:var(--noteink);font-size:15px;font-weight:800;padding:14px 12px 13px;text-align:left}
.ac2 .ac2-nb::after{content:" +";font-weight:900}
.ac2-note.ac2-open .ac2-nb::after{content:" \2212"}
.ac2 .ac2-nc{padding:0 14px 14px}
.ac2 .ac2-nc[hidden]{display:none}
.ac2 p.ac2-ct{font-size:13.5px;line-height:1.5;color:var(--noteink);overflow-wrap:anywhere}
.ac2 .ac2-copy{margin-top:10px;border:2px solid var(--noteink);background:transparent;color:var(--noteink);font-size:13px;font-weight:800;border-radius:999px;padding:3px 12px}
.ac2 .ac2-copy:hover{background:var(--noteink);color:var(--note)}
.ac2 .ac2-nb:focus-visible,.ac2 .ac2-copy:focus-visible,.ac2 a.ac2-doi:focus-visible{outline:3px solid var(--blue);outline-offset:2px}
@media (max-width:600px){
.ac2-desk{padding:30px 12px 36px;border-radius:20px;gap:44px}
.ac2-page{padding:38px 18px 18px}
.ac2-p0{transform:rotate(-.6deg)}
.ac2-p1{transform:rotate(.5deg)}
.ac2 p.ac2-band{padding-right:0;font-size:11.5px}
.ac2-note{top:-20px;right:12px;width:108px}
.ac2-note.ac2-open{width:calc(100% - 24px)}
.ac2 h2.ac2-t{font-size:22px;margin-top:18px}
.ac2-p0 h2.ac2-t{padding-right:0}
.ac2-stamp{position:relative;top:auto;right:auto;display:inline-block;margin-top:18px;transform:rotate(-4deg)}
@keyframes ac2stamp{0%{opacity:0;transform:rotate(-12deg) scale(2)}60%{opacity:.95;transform:rotate(-3deg) scale(.95)}100%{opacity:.9;transform:rotate(-4deg) scale(1)}}
.ac2-stamp span{font-size:12px;padding:6px 10px}
.ac2-stamp span br{display:none}
.ac2 p.ac2-abs{column-count:1}
.ac2-foot{font-size:12.5px}
}
@media (prefers-reduced-motion:reduce){.ac2 *{animation:none!important;transition:none!important}.ac2-stamp{opacity:.9}}
</style>
<div class="ac2">
<header class="ac2-mast"><h1 class="ac2-h1">Academia</h1></header>
<div class="ac2-desk">
<article class="ac2-page ac2-p0">
<div class="ac2-note"><button type="button" class="ac2-nb" aria-expanded="false" aria-controls="ac2-c0">Cite this</button><div class="ac2-nc" id="ac2-c0" hidden><p class="ac2-ct">Sodacı, H., &amp; Küntay, A. C. (2026). Real-time speech adaptation to human and robot audiences. Companion Proceedings of the 21st ACM/IEEE International Conference on Human-Robot Interaction, HRI Companion &#39;26, 392-396. https://doi.org/10.1145/3776734.3794422</p><button type="button" class="ac2-copy" data-apa="Sodacı, H., &amp; Küntay, A. C. (2026). Real-time speech adaptation to human and robot audiences. Companion Proceedings of the 21st ACM/IEEE International Conference on Human-Robot Interaction, HRI Companion &#39;26, 392-396. https://doi.org/10.1145/3776734.3794422">Copy</button></div></div>
<p class="ac2-band">Companion Proceedings of the 21st ACM/IEEE International Conference on Human-Robot Interaction (HRI Companion ’26) · 392–396 · 2026</p>
<div class="ac2-stamp" aria-label="Honorable Mention Award"><span>Honorable Mention <br>Award</span></div><h2 class="ac2-t">Real-Time Speech Adaptation to Human and Robot Audiences</h2>
<p class="ac2-au"><strong>Sodacı, H.</strong>, &amp; Küntay, A. C.</p>
<div class="ac2-absw"><p class="ac2-lab">Abstract</p><p class="ac2-abs">Audience design (adapting communication to an audience&#39;s needs and shared knowledge) poses unique challenges in human-robot interaction (HRI), where speakers lack prior experience with robots and must rely on real-time communicative cues. In a word-guessing game, participants described words to either a robot or a human audience, who guessed the words with a 25% error rate. Descriptions were coded for the number of semantic details (distinct meaning-relevant units). Participants produced more semantic details for robots than humans, with a marginal trend suggesting speakers reduced details for humans but maintained elaboration for robots during consistent success. This asymmetry hints at persistent assumptions about robot competence that behavioral success may not override.</p></div>
<p class="ac2-kw"><span class="ac2-lab">Keywords</span>Social robots, Audience design, Speech adaptation, Task-based interaction</p>
<div class="ac2-foot"><a class="ac2-doi" href="https://doi.org/10.1145/3776734.3794422" target="_blank" rel="noopener">doi.org/10.1145/3776734.3794422</a><span class="ac2-pn">392</span></div>
</article>
<article class="ac2-page ac2-p1">
<div class="ac2-note"><button type="button" class="ac2-nb" aria-expanded="false" aria-controls="ac2-c1">Cite this</button><div class="ac2-nc" id="ac2-c1" hidden><p class="ac2-ct">Leeuwestein, H., Barking, M., Sodacı, H., Oudgenoeg-Paz, O., Verhagen, J., Vogt, P., Aarts, R., Spit, S., de Haas, M., de Wit, J., &amp; Leseman, P. (2020). Teaching Turkish-Dutch kindergartners Dutch vocabulary with a social robot: Does the robot&#39;s use of Turkish translations benefit children&#39;s Dutch vocabulary learning? Journal of Computer Assisted Learning, 37(3), 603-620. https://doi.org/10.1111/jcal.12510</p><button type="button" class="ac2-copy" data-apa="Leeuwestein, H., Barking, M., Sodacı, H., Oudgenoeg-Paz, O., Verhagen, J., Vogt, P., Aarts, R., Spit, S., de Haas, M., de Wit, J., &amp; Leseman, P. (2020). Teaching Turkish-Dutch kindergartners Dutch vocabulary with a social robot: Does the robot&#39;s use of Turkish translations benefit children&#39;s Dutch vocabulary learning? Journal of Computer Assisted Learning, 37(3), 603-620. https://doi.org/10.1111/jcal.12510">Copy</button></div></div>
<p class="ac2-band">Journal of Computer Assisted Learning, 37(3) · 603–620 · 2020</p>
<h2 class="ac2-t">Teaching Turkish–Dutch kindergartners Dutch vocabulary with a social robot: Does the robot’s use of Turkish translations benefit children’s Dutch vocabulary learning?</h2>
<p class="ac2-au">Leeuwestein, H., Barking, M., <strong>Sodacı, H.</strong>, Oudgenoeg-Paz, O., Verhagen, J., Vogt, P., Aarts, R., Spit, S., de Haas, M., de Wit, J., &amp; Leseman, P.</p>
<div class="ac2-absw"><p class="ac2-lab">Abstract</p><p class="ac2-abs">Providing first language (L1) translations in L2 vocabulary interventions may be beneficial for L2 vocabulary learning. However, in linguistically diverse L2 classrooms, teachers cannot provide L1 translations to all children. Social robots do offer such opportunities, as they can be programmed to speak any combination of languages. This study investigates whether providing L1 translations in a robot-assisted L2 vocabulary training facilitates children&#39;s learning. Participants were Turkish-Dutch kindergartners (n = 67) who were taught six Dutch (L2) words for which they knew the L1 (Turkish), but not the L2 Dutch form. Half of these words were taught by a Turkish-Dutch bilingual robot, alongside their Turkish translations; the other half by a monolingual Dutch robot. Results indicated better performance in the Dutch-only condition than in the Turkish-Dutch condition. The majority of children preferred working with the bilingual robot, but children&#39;s preference did not affect word learning. Contrary to the prediction, the study found no evidence for a facilitating effect of providing L1 translations through a robot on bilingual children&#39;s L2 word learning.</p></div>
<p class="ac2-kw"><span class="ac2-lab">Keywords</span>First language translations, Kindergartners, Robot-assisted language learning, Second language, Vocabulary</p>
<div class="ac2-foot"><a class="ac2-doi" href="https://doi.org/10.1111/jcal.12510" target="_blank" rel="noopener">doi.org/10.1111/jcal.12510</a><span class="ac2-pn">603</span></div>
</article>
</div>
</div>
<script>
(function(){
var R=document.querySelector('.ac2');
if(!R)return;
function fallback(t){var a=document.createElement('textarea');a.value=t;a.style.position='fixed';a.style.opacity='0';document.body.appendChild(a);a.select();try{document.execCommand('copy');}catch(e){}document.body.removeChild(a);}
R.querySelectorAll('.ac2-nb').forEach(function(b){b.addEventListener('click',function(){
var note=b.parentNode,box=document.getElementById(b.getAttribute('aria-controls')),open=b.getAttribute('aria-expanded')!=='true';
b.setAttribute('aria-expanded',open?'true':'false');note.classList.toggle('ac2-open',open);box.hidden=!open;
});});
R.querySelectorAll('.ac2-copy').forEach(function(b){b.addEventListener('click',function(){
var t=b.getAttribute('data-apa');
function ok(){b.textContent='Copied ✓';setTimeout(function(){b.textContent='Copy';},1800);}
if(navigator.clipboard&&navigator.clipboard.writeText){navigator.clipboard.writeText(t).then(ok,function(){fallback(t);ok();});}else{fallback(t);ok();}
});});
var st=R.querySelectorAll('.ac2-stamp');
if('IntersectionObserver' in window){
var io=new IntersectionObserver(function(es){es.forEach(function(en){if(en.isIntersecting){setTimeout(function(){en.target.classList.add('ac2-in');},250);io.unobserve(en.target);}});},{threshold:.6});
st.forEach(function(s){io.observe(s);});
}else{st.forEach(function(s){s.classList.add('ac2-in');});}
})();
</script>
