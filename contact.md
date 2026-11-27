---
title: Contact
permalink: /contact/
layout: page
excerpt: Get in touch with Hande Sodacı.
comments: false
---
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Figtree:wght@400;500;600;700;800;900&display=swap" rel="stylesheet">
<style>
.header:has(+ .page-content .ctc){display:none}
.ctc{--ink:#1d1b26;--muted:#6a6878;--card:#f5f2ec;--field:#ffffff;--line:rgba(29,27,38,.14);--acc:#3b6fe0;--acc-s:#dce6fb}
body[data-theme="dark"] .ctc{--ink:#efece6;--muted:#a6a3b0;--card:#24232c;--field:#2f2e38;--line:rgba(255,255,255,.14);--acc:#8aaeff;--acc-s:#2b3a5e}
.ctc{font-family:"Figtree",system-ui,-apple-system,"Segoe UI",sans-serif;color:var(--ink);padding:4px 0 40px}
.ctc *{box-sizing:border-box}
.ctc p{margin:0}
.ctc h1.ctc-h1{font-family:inherit;font-size:clamp(44px,9vw,72px);font-weight:800;letter-spacing:-.035em;line-height:1;margin:0 0 16px;color:var(--ink)}
.ctc h1.ctc-h1 span{color:var(--acc)}
.ctc p.ctc-lead{font-size:18px;line-height:1.6;max-width:540px;margin-bottom:28px;color:var(--ink)}
.ctc-card{background:var(--card);border-radius:22px;padding:28px 28px 26px;max-width:620px}
.ctc-field{display:flex;flex-direction:column;gap:7px;margin-bottom:18px}
.ctc label{font-size:14px;font-weight:700;color:var(--ink)}
.ctc input[type="text"],.ctc input[type="email"],.ctc textarea{width:100%;font-family:inherit;font-size:16px;color:var(--ink);background:var(--field);border:2px solid var(--line);border-radius:12px;padding:11px 14px;line-height:1.5;transition:border-color .2s,box-shadow .2s;margin:0}
.ctc textarea{resize:vertical;min-height:150px}
.ctc input::placeholder,.ctc textarea::placeholder{color:var(--muted);opacity:.75}
.ctc input:focus,.ctc textarea:focus{outline:none;border-color:var(--acc);box-shadow:0 0 0 4px var(--acc-s)}
.ctc button.ctc-send{font-family:inherit;font-size:16px;font-weight:700;color:var(--card);background:var(--ink);border:0;border-radius:999px;padding:12px 26px;cursor:pointer;margin-top:4px;transition:transform .2s,opacity .2s}
.ctc button.ctc-send:hover{transform:translateY(-2px)}
.ctc button:focus-visible{outline:3px solid var(--acc);outline-offset:3px}
.ctc-ov{position:fixed;inset:0;z-index:100;display:flex;align-items:center;justify-content:center;padding:20px;background:rgba(15,14,20,.55)}
.ctc-ov[hidden]{display:none}
.ctc-modal{background:var(--card);color:var(--ink);border-radius:20px;padding:28px 30px 24px;max-width:360px;width:100%;text-align:center;box-shadow:0 30px 60px -30px rgba(0,0,0,.6)}
.ctc p.ctc-mt{font-size:22px;font-weight:800;letter-spacing:-.01em;margin-bottom:18px}
.ctc .ctc-close{font-family:inherit;font-size:15px;font-weight:700;color:var(--ink);background:transparent;border:2px solid var(--line);border-radius:999px;padding:8px 20px;cursor:pointer}
.ctc .ctc-close:hover{border-color:var(--ink)}
@media (max-width:600px){.ctc-card{padding:20px 16px 18px;border-radius:18px}.ctc p.ctc-lead{font-size:17px}}
.ctc p.ctc-lead{margin-bottom:22px}
.ctc-card{position:relative;margin-top:84px}
.ctc-form{position:relative}
.ctc-bot{position:absolute;right:46px;bottom:calc(100% - 8px);width:120px;height:100px;z-index:2;pointer-events:none}
.ctc .ctc-rb{display:block;width:120px;height:100px;overflow:visible}
.ctc .ctc-ant{fill:#13a184;transition:fill .2s}
.ctc .ctc-hand{fill:#13a184}
.ctc .ctc-head{transition:transform .25s cubic-bezier(.3,1.6,.5,1)}
.ctc-bot.ctc-bob .ctc-head{transform:translateY(2px)}
.ctc-bot.ctc-bob .ctc-ant{fill:#ffcd55}
.ctc .ctc-eyes{transition:transform .35s cubic-bezier(.3,.8,.3,1)}
.ctc .ctc-eye{transform-box:fill-box;transform-origin:center}
.ctc-bot.ctc-blink .ctc-eye{transform:scaleY(.1)}
.ctc .ctc-happy,.ctc .ctc-m2{opacity:0;transition:opacity .2s}
.ctc .ctc-m1,.ctc .ctc-eyes{transition:opacity .2s,transform .35s cubic-bezier(.3,.8,.3,1)}
.ctc-bot.ctc-joy .ctc-happy,.ctc-bot.ctc-joy .ctc-m2{opacity:1}
.ctc-bot.ctc-joy .ctc-eyes,.ctc-bot.ctc-joy .ctc-m1{opacity:0}
.ctc p.ctc-bub{position:absolute;right:calc(100% + 6px);top:26px;white-space:nowrap;background:var(--ink);color:var(--card);font-size:14px;font-weight:700;padding:7px 13px;border-radius:14px 14px 4px 14px;opacity:0;transform:translateY(6px) scale(.96);transform-origin:right bottom;transition:opacity .25s,transform .25s}
.ctc p.ctc-bub.ctc-on{opacity:1;transform:none}
.ctc .ctc-env{position:absolute;left:60px;bottom:10px;width:40px;height:28px;opacity:0;pointer-events:none}
.ctc-form.ctc-fly .ctc-env{animation:ctcfly 1s cubic-bezier(.4,.1,.3,1) forwards}
@keyframes ctcfly{0%{opacity:0;transform:translate(0,0) rotate(0)}15%{opacity:1}100%{opacity:0;transform:translate(380px,-330px) rotate(-18deg) scale(.6)}}
.ctc .ctc-mbot{display:block;width:110px;height:86px;margin:-6px auto 10px;overflow:visible}
.ctc .ctc-wave{transform-origin:110px 64px;animation:ctcwave 1s ease-in-out 3}
@keyframes ctcwave{0%,100%{transform:rotate(0)}25%{transform:rotate(-22deg)}75%{transform:rotate(14deg)}}
@media (max-width:600px){.ctc-bot{right:18px;transform:scale(.85);transform-origin:right bottom}.ctc-card{margin-top:74px}.ctc p.ctc-bub{font-size:13px}@keyframes ctcfly{0%{opacity:0;transform:translate(0,0)}15%{opacity:1}100%{opacity:0;transform:translate(200px,-420px) rotate(-18deg) scale(.6)}}}
@media (prefers-reduced-motion:reduce){.ctc *{animation:none!important;transition:none!important}}
</style>
<div class="ctc">
<h1 class="ctc-h1">Contact<span>.</span></h1>
<p class="ctc-lead">Have a question, an opportunity, or just want to say hi? Send a message below and I will get back to you as soon as possible.</p>
<div class="ctc-card">
<div class="ctc-bot" aria-hidden="true"><p class="ctc-bub"></p><svg class="ctc-rb" viewBox="0 0 120 100"><g class="ctc-head"><path d="M60 22V11" stroke="#9aa7ad" stroke-width="3"/><circle class="ctc-ant" cx="60" cy="8" r="5.5"/><rect x="13" y="39" width="10" height="20" rx="4" fill="#9aa7ad"/><rect x="97" y="39" width="10" height="20" rx="4" fill="#9aa7ad"/><rect x="21" y="21" width="78" height="57" rx="19" fill="#eef2f3" stroke="#c5cfd3" stroke-width="1.5"/><circle cx="34" cy="62" r="5" fill="#ff8f7d" opacity=".35"/><circle cx="86" cy="62" r="5" fill="#ff8f7d" opacity=".35"/><g class="ctc-eyes"><g class="ctc-eye"><circle cx="45" cy="47" r="8.5" fill="#1d1b26"/><circle cx="48" cy="44" r="2.6" fill="#fff"/></g><g class="ctc-eye"><circle cx="75" cy="47" r="8.5" fill="#1d1b26"/><circle cx="78" cy="44" r="2.6" fill="#fff"/></g></g><g class="ctc-happy" fill="none" stroke="#1d1b26" stroke-width="3.5" stroke-linecap="round"><path d="M38 49Q45 40 52 49"/><path d="M68 49Q75 40 82 49"/></g><path class="ctc-m1" d="M52 63Q60 69 68 63" fill="none" stroke="#1d1b26" stroke-width="2.6" stroke-linecap="round"/><path class="ctc-m2" d="M50 61Q60 73 70 61Z" fill="#1d1b26"/></g><rect x="52" y="77" width="16" height="15" fill="#9aa7ad"/><rect class="ctc-hand" x="27" y="86" width="22" height="14" rx="7"/><rect class="ctc-hand" x="71" y="86" width="22" height="14" rx="7"/></svg></div>
<form action="https://formsubmit.co/handesodaci@gmail.com" method="POST" class="ctc-form">
<input type="hidden" name="_subject" value="New message from hsodaci.github.io">
<input type="text" name="_honey" style="display:none" tabindex="-1" autocomplete="off">
<input type="hidden" name="_captcha" value="false">
<input type="hidden" name="_next" value="{{ site.url }}/contact/?sent=true">
<div class="ctc-field"><label for="name">Your name</label><input type="text" id="name" name="name" placeholder="Jane Doe" autocomplete="name" required></div>
<div class="ctc-field"><label for="email">Email address</label><input type="email" id="email" name="email" placeholder="jane@example.com" autocomplete="email" required></div>
<div class="ctc-field"><label for="message">Message</label><textarea id="message" name="message" rows="6" placeholder="What can I help with?" required></textarea></div>
<button type="submit" class="ctc-send">Send message</button><svg class="ctc-env" viewBox="0 0 40 28" aria-hidden="true"><rect x="1" y="1" width="38" height="26" rx="4" fill="#fff" stroke="#1d1b26" stroke-width="2"/><path d="M3 4L20 16L37 4" fill="none" stroke="#1d1b26" stroke-width="2" stroke-linejoin="round"/></svg>
</form>
</div>
<div id="contact-sent-overlay" class="ctc-ov" hidden>
<div class="ctc-modal" role="dialog" aria-modal="true" aria-labelledby="contact-sent-title">
<svg class="ctc-mbot" viewBox="0 0 140 110" aria-hidden="true"><g class="ctc-wave"><rect x="104" y="34" width="12" height="30" rx="6" fill="#13a184"/><circle cx="110" cy="32" r="9" fill="#13a184"/></g><path d="M60 22V11" stroke="#9aa7ad" stroke-width="3"/><circle cx="60" cy="8" r="5.5" fill="#13a184"/><rect x="13" y="39" width="10" height="20" rx="4" fill="#9aa7ad"/><rect x="97" y="39" width="10" height="20" rx="4" fill="#9aa7ad"/><rect x="21" y="21" width="78" height="57" rx="19" fill="#eef2f3" stroke="#c5cfd3" stroke-width="1.5"/><circle cx="34" cy="62" r="5" fill="#ff8f7d" opacity=".45"/><circle cx="86" cy="62" r="5" fill="#ff8f7d" opacity=".45"/><g fill="none" stroke="#1d1b26" stroke-width="3.5" stroke-linecap="round"><path d="M38 49Q45 40 52 49"/><path d="M68 49Q75 40 82 49"/></g><path d="M50 61Q60 73 70 61Z" fill="#1d1b26"/><rect x="52" y="77" width="16" height="10" fill="#9aa7ad"/><rect x="34" y="86" width="52" height="24" rx="10" fill="#13a184"/></svg>
<p id="contact-sent-title" class="ctc-mt">Message received</p>
<button type="button" id="contact-sent-close" class="ctc-close">Close</button>
</div>
</div>
</div>
<script>
(function(){
var C=document.querySelector('.ctc');
if(!C)return;
var bot=C.querySelector('.ctc-bot'),eyes=C.querySelector('.ctc-eyes'),bub=C.querySelector('.ctc-bub'),form=C.querySelector('.ctc-form');
if(!bot||!form)return;
var reduce=window.matchMedia&&window.matchMedia('(prefers-reduced-motion: reduce)').matches;
var focused=null,bubT=null,saidName='',saidMsg=false,bobT=null;
function look(dx,dy){eyes.style.transform='translate('+dx.toFixed(2)+'px,'+dy.toFixed(2)+'px)';}
function lookAt(x,y){var r=bot.getBoundingClientRect(),cx=r.left+r.width/2,cy=r.top+r.height*.47,vx=x-cx,vy=y-cy,d=Math.sqrt(vx*vx+vy*vy)||1;look(vx/d*4.5,vy/d*3.5);}
function lookField(el){var r=el.getBoundingClientRect(),len=(el.value||'').length,x=el.tagName==='TEXTAREA'?r.left+Math.min(r.width*.6,40+len*2):r.left+Math.min(r.width-16,16+len*8.5),y=el.tagName==='TEXTAREA'?r.top+Math.min(r.height-20,24+len*.25):r.top+r.height/2;lookAt(x,y);}
function say(t,ms){bub.textContent=t;bub.classList.add('ctc-on');clearTimeout(bubT);bubT=setTimeout(function(){bub.classList.remove('ctc-on');},ms||2600);}
function joy(ms){bot.classList.add('ctc-joy');setTimeout(function(){bot.classList.remove('ctc-joy');},ms||1400);}
form.addEventListener('focusin',function(e){if(e.target.matches('input[type="text"]:not([name="_honey"]),input[type="email"],textarea')){focused=e.target;lookField(focused);}});
form.addEventListener('focusout',function(e){
var el=e.target;
setTimeout(function(){if(!form.contains(document.activeElement)||document.activeElement.tagName==='BUTTON'){focused=null;look(0,0);}},10);
if(el.name==='name'){var n=(el.value||'').trim().split(/\s+/)[0];if(n&&n!==saidName){saidName=n;say('Nice to meet you, '+n.slice(0,18)+'!');joy(1500);}}
});
form.addEventListener('input',function(e){
var el=e.target;if(el===focused)lookField(el);
if(!reduce){bot.classList.add('ctc-bob');clearTimeout(bobT);bobT=setTimeout(function(){bot.classList.remove('ctc-bob');},120);}
if(el.name==='message'&&!saidMsg&&el.value.length>24){saidMsg=true;say('I\u2019m listening.');}
});
function blink(){bot.classList.add('ctc-blink');setTimeout(function(){bot.classList.remove('ctc-blink');},140);setTimeout(blink,2600+Math.random()*3800);}
setTimeout(blink,1800);
function glance(){if(!focused&&!bot.classList.contains('ctc-joy')){var a=Math.random()*Math.PI*2;look(Math.cos(a)*3.5,Math.sin(a)*2.5);setTimeout(function(){if(!focused)look(0,0);},900);}setTimeout(glance,4200+Math.random()*4000);}
setTimeout(glance,3500);
var sending=false;
form.addEventListener('submit',function(e){
if(sending)return;
var hp=form.querySelector('[name="_honey"]');if(hp&&hp.value)return;
e.preventDefault();sending=true;
bot.classList.add('ctc-joy');say('On its way!',3000);
if(!reduce)form.classList.add('ctc-fly');
setTimeout(function(){HTMLFormElement.prototype.submit.call(form);},reduce?300:1000);
});
})();
(function(){
if(window.location.search.indexOf('sent=true')<0)return;
var overlay=document.getElementById('contact-sent-overlay'),closeBtn=document.getElementById('contact-sent-close');
function closeModal(){overlay.hidden=true;var url=new URL(window.location.href);url.searchParams.delete('sent');window.history.replaceState({},'',url);}
overlay.hidden=false;closeBtn.focus();
closeBtn.addEventListener('click',closeModal);
overlay.addEventListener('click',function(e){if(e.target===overlay)closeModal();});
document.addEventListener('keydown',function(e){if(e.key==='Escape')closeModal();});
})();
</script>
<!--
  This form uses FormSubmit (https://formsubmit.co) to relay submissions to
  handesodaci@gmail.com without needing a backend server. The FIRST
  submission after this page goes live will trigger a one-time confirmation
  email from FormSubmit to handesodaci@gmail.com. You must click the
  activation link in that email before the form will actually deliver
  messages.
-->
