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
.ctc-bot{position:absolute;right:46px;bottom:100%;width:120px;height:92px;z-index:2}
.ctc-win{position:absolute;left:-40px;right:-40px;top:-40px;bottom:0;overflow:hidden;pointer-events:none}
.ctc .ctc-rb{position:absolute;left:40px;bottom:0;display:block;width:120px;height:92px;transform:translateY(105%);transition:transform .55s cubic-bezier(.3,1.5,.5,1)}
.ctc-bot.ctc-up .ctc-rb{transform:translateY(0)}
.ctc-bot.ctc-up.ctc-shy .ctc-rb{transform:translateY(46%);transition-duration:.3s}
.ctc-bot.ctc-up.ctc-bob .ctc-rb{transform:translateY(3px);transition-duration:.12s}
.ctc .ctc-ant{fill:#13a184;transition:fill .2s}
.ctc-bot.ctc-bob .ctc-ant{fill:#ffcd55}
.ctc .ctc-hands{position:absolute;left:0;bottom:-12px;width:120px;height:20px;overflow:visible;pointer-events:none}
.ctc .ctc-hands rect{fill:#13a184}
.ctc .ctc-hl,.ctc .ctc-hr{transform-box:fill-box;transform-origin:50% 50%;transform:translateY(12px);opacity:0;transition:transform .35s cubic-bezier(.3,1.5,.5,1),opacity .2s}
.ctc-bot.ctc-grip .ctc-hl,.ctc-bot.ctc-grip .ctc-hr{transform:none;opacity:1}
.ctc-bot.ctc-grip.ctc-tapl .ctc-hl,.ctc-bot.ctc-grip.ctc-tapr .ctc-hr{transform:translateY(-4px);transition-duration:.08s}
.ctc-bot.ctc-grip.ctc-wave .ctc-hr{animation:ctchwave 1.3s ease-in-out}
@keyframes ctchwave{0%{transform:none}20%{transform:translate(30px,-40px) rotate(-20deg)}35%{transform:translate(30px,-40px) rotate(18deg)}50%{transform:translate(30px,-40px) rotate(-18deg)}65%{transform:translate(30px,-40px) rotate(14deg)}82%{transform:translate(30px,-40px) rotate(0)}100%{transform:none}}
.ctc-bot.ctc-grip.ctc-wind .ctc-hr{transform:translate(34px,-52px) rotate(-30deg);transition-duration:.3s}
.ctc-bot.ctc-grip.ctc-throw .ctc-hr{transform:translate(4px,-74px) rotate(25deg);transition:transform .16s ease-out}
.ctc .ctc-eyes{transition:transform .3s cubic-bezier(.3,.8,.3,1),opacity .2s}
.ctc-bot.ctc-track .ctc-eyes{transition:opacity .2s}
.ctc .ctc-eye{transform-box:fill-box;transform-origin:center}
.ctc-bot.ctc-blink .ctc-eye{transform:scaleY(.1)}
.ctc .ctc-happy,.ctc .ctc-m2,.ctc .ctc-m3{opacity:0;transition:opacity .2s}
.ctc .ctc-m1{transition:opacity .2s}
.ctc-bot.ctc-joy .ctc-happy,.ctc-bot.ctc-joy .ctc-m2{opacity:1}
.ctc-bot.ctc-joy .ctc-eyes,.ctc-bot.ctc-joy .ctc-m1,.ctc-bot.ctc-shy .ctc-m1{opacity:0}
.ctc-bot.ctc-shy:not(.ctc-joy) .ctc-m3{opacity:1}
.ctc p.ctc-bub{position:absolute;right:calc(100% + 4px);top:22px;white-space:nowrap;background:var(--ink);color:var(--card);font-size:14px;font-weight:700;padding:7px 13px;border-radius:14px 14px 4px 14px;opacity:0;transform:translateY(6px) scale(.96);transform-origin:right bottom;transition:opacity .25s,transform .25s;pointer-events:none}
.ctc p.ctc-bub.ctc-on{opacity:1;transform:none}
.ctc-sheet{position:fixed;z-index:60;border-radius:12px;background:#fff;box-shadow:0 10px 24px -12px rgba(0,0,0,.45);transform-origin:0 0;pointer-events:none;background-image:repeating-linear-gradient(transparent 0 26px,#dfe4ec 26px 28px);background-position:0 18px}
.ctc-plane{position:fixed;z-index:61;width:40px;height:28px;margin:-14px 0 0 -20px;pointer-events:none;filter:drop-shadow(0 6px 6px rgba(0,0,0,.25))}
.ctc-plane svg{display:block;width:40px;height:28px}
.ctc-trail{position:fixed;z-index:59;width:1px;height:1px;overflow:visible;pointer-events:none}
.ctc-form.ctc-taken textarea{color:transparent;transition:color .3s}
.ctc .ctc-mbot{display:block;width:110px;height:86px;margin:-6px auto 10px;overflow:visible}
.ctc .ctc-wave{transform-origin:110px 64px;animation:ctcwave 1s ease-in-out 3}
@keyframes ctcwave{0%,100%{transform:rotate(0)}25%{transform:rotate(-22deg)}75%{transform:rotate(14deg)}}
@media (max-width:600px){.ctc-bot{right:16px;transform:scale(.85);transform-origin:right bottom}.ctc-card{margin-top:74px}.ctc p.ctc-bub{font-size:13px}}
@media (prefers-reduced-motion:reduce){.ctc *{animation:none!important;transition:none!important}}
</style>
<div class="ctc">
<h1 class="ctc-h1">Contact<span>.</span></h1>
<p class="ctc-lead">Have a question, an opportunity, or just want to say hi? Send a message below and I will get back to you as soon as possible.</p>
<div class="ctc-card">
<div class="ctc-bot" aria-hidden="true"><p class="ctc-bub"></p><div class="ctc-win"><svg class="ctc-rb" viewBox="0 0 120 92"><path d="M60 22V11" stroke="#9aa7ad" stroke-width="3"/><circle class="ctc-ant" cx="60" cy="8" r="5.5"/><rect x="13" y="39" width="10" height="20" rx="4" fill="#9aa7ad"/><rect x="97" y="39" width="10" height="20" rx="4" fill="#9aa7ad"/><rect x="21" y="21" width="78" height="57" rx="19" fill="#eef2f3" stroke="#c5cfd3" stroke-width="1.5"/><circle cx="34" cy="62" r="5" fill="#ff8f7d" opacity=".35"/><circle cx="86" cy="62" r="5" fill="#ff8f7d" opacity=".35"/><g class="ctc-eyes"><g class="ctc-eye"><circle cx="45" cy="47" r="8.5" fill="#1d1b26"/><circle cx="48" cy="44" r="2.6" fill="#fff"/></g><g class="ctc-eye"><circle cx="75" cy="47" r="8.5" fill="#1d1b26"/><circle cx="78" cy="44" r="2.6" fill="#fff"/></g></g><g class="ctc-happy" fill="none" stroke="#1d1b26" stroke-width="3.5" stroke-linecap="round"><path d="M38 49Q45 40 52 49"/><path d="M68 49Q75 40 82 49"/></g><path class="ctc-m1" d="M52 63Q60 69 68 63" fill="none" stroke="#1d1b26" stroke-width="2.6" stroke-linecap="round"/><path class="ctc-m2" d="M50 61Q60 73 70 61Z" fill="#1d1b26"/><path class="ctc-m3" d="M54 64Q57 61 60 64Q63 67 66 64" fill="none" stroke="#1d1b26" stroke-width="2.4" stroke-linecap="round"/><rect x="52" y="77" width="16" height="15" fill="#9aa7ad"/></svg></div><svg class="ctc-hands" viewBox="0 0 120 20"><g class="ctc-hl"><rect x="27" y="2" width="22" height="14" rx="7"/></g><g class="ctc-hr"><rect x="71" y="2" width="22" height="14" rx="7"/></g></svg></div>
<form action="https://formsubmit.co/handesodaci@gmail.com" method="POST" class="ctc-form">
<input type="hidden" name="_subject" value="New message from hsodaci.github.io">
<input type="text" name="_honey" style="display:none" tabindex="-1" autocomplete="off">
<input type="hidden" name="_captcha" value="false">
<input type="hidden" name="_next" value="{{ site.url }}/contact/?sent=true">
<div class="ctc-field"><label for="name">Your name</label><input type="text" id="name" name="name" placeholder="Jane Doe" autocomplete="name" required></div>
<div class="ctc-field"><label for="email">Email address</label><input type="email" id="email" name="email" placeholder="jane@example.com" autocomplete="email" required></div>
<div class="ctc-field"><label for="message">Message</label><textarea id="message" name="message" rows="6" placeholder="What can I help with?" required></textarea></div>
<button type="submit" class="ctc-send">Send message</button>
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
var bot=C.querySelector('.ctc-bot'),eyes=C.querySelector('.ctc-eyes'),bub=C.querySelector('.ctc-bub'),form=C.querySelector('.ctc-form'),hr=C.querySelector('.ctc-hr');
if(!bot||!form)return;
var reduce=window.matchMedia&&window.matchMedia('(prefers-reduced-motion: reduce)').matches;
var focused=null,bubT=null,saidName='',saidMsg=false,bobT=null,tapSide=0,busy=false,shy=false,shyT=null;
var PLANE='<svg viewBox="0 0 40 28"><path d="M1 13L39 1L27 27L19 17Z" fill="#fff" stroke="#1d1b26" stroke-width="1.8" stroke-linejoin="round"/><path d="M39 1L19 17L17 26L23 20" fill="#e6ebf2" stroke="#1d1b26" stroke-width="1.8" stroke-linejoin="round"/></svg>';
function look(dx,dy){eyes.style.transform='translate('+dx.toFixed(2)+'px,'+dy.toFixed(2)+'px)';}
function lookAt(x,y){var r=bot.getBoundingClientRect(),cx=r.left+r.width/2,cy=r.top+r.height*.5,vx=x-cx,vy=y-cy,d=Math.sqrt(vx*vx+vy*vy)||1,k=Math.min(1,d/120);look(vx/d*4.8*k,vy/d*3.6*k);}
function lookField(el){var r=el.getBoundingClientRect(),len=(el.value||'').length,ta=el.tagName==='TEXTAREA',x=ta?r.left+Math.min(r.width*.6,40+len*2):r.left+Math.min(r.width-16,16+len*8.5),y=ta?r.top+Math.min(r.height-20,24+len*.25):r.top+r.height/2;lookAt(x,y);}
function say(t,ms){bub.textContent=t;bub.classList.add('ctc-on');clearTimeout(bubT);bubT=setTimeout(function(){bub.classList.remove('ctc-on');},ms||2600);}
function joy(ms){bot.classList.add('ctc-joy');setTimeout(function(){if(!busy)bot.classList.remove('ctc-joy');},ms||1400);}
function wave(){bot.classList.remove('ctc-wave');void bot.offsetWidth;bot.classList.add('ctc-wave');setTimeout(function(){bot.classList.remove('ctc-wave');},1350);}
function enter(){bot.classList.add('ctc-up');setTimeout(function(){bot.classList.add('ctc-grip');},380);}
if(reduce){bot.classList.add('ctc-up','ctc-grip');}else{setTimeout(enter,650);}
document.addEventListener('mousemove',function(e){
if(busy||reduce||!bot.classList.contains('ctc-grip'))return;
var r=bot.getBoundingClientRect(),cx=r.left+r.width/2,cy=r.top+r.height/2,dx=e.clientX-cx,dy=e.clientY-cy,d=Math.sqrt(dx*dx+dy*dy);
if(!focused)lookAt(e.clientX,e.clientY);
if(d<85&&!shy){shy=true;clearTimeout(shyT);bot.classList.add('ctc-shy');}
else if(d>150&&shy){clearTimeout(shyT);shyT=setTimeout(function(){shy=false;bot.classList.remove('ctc-shy');},350);}
},{passive:true});
form.addEventListener('focusin',function(e){if(e.target.matches('input[type="text"]:not([name="_honey"]),input[type="email"],textarea')){focused=e.target;lookField(focused);}});
form.addEventListener('focusout',function(e){
var el=e.target;
setTimeout(function(){var a=document.activeElement;if(!form.contains(a)||a.tagName==='BUTTON'){focused=null;if(!busy)look(0,0);}},10);
if(el.name==='name'){var n=(el.value||'').trim().split(/\s+/)[0];if(n&&n!==saidName){saidName=n;say('Nice to meet you, '+n.slice(0,18)+'!');joy(1500);if(!reduce)wave();}}
});
form.addEventListener('input',function(e){
var el=e.target;if(el===focused)lookField(el);
if(!reduce&&!busy){var side=(tapSide++%2)?'ctc-tapr':'ctc-tapl';bot.classList.remove('ctc-tapl','ctc-tapr');bot.classList.add('ctc-bob',side);clearTimeout(bobT);bobT=setTimeout(function(){bot.classList.remove('ctc-bob','ctc-tapl','ctc-tapr');},110);}
if(el.name==='message'&&!saidMsg&&el.value.length>24){saidMsg=true;say('I’m listening.');}
});
function blink(){if(!bot.classList.contains('ctc-joy')){bot.classList.add('ctc-blink');setTimeout(function(){bot.classList.remove('ctc-blink');},140);}setTimeout(blink,2600+Math.random()*3800);}
setTimeout(blink,2200);
function glance(){if(!focused&&!busy&&!shy){var a=Math.random()*Math.PI*2;look(Math.cos(a)*3.5,Math.sin(a)*2.5);setTimeout(function(){if(!focused&&!busy)look(0,0);},900);}setTimeout(glance,4800+Math.random()*4000);}
setTimeout(glance,4000);
function el(tag,cls,html){var x=document.createElement(tag);x.className=cls;if(html)x.innerHTML=html;document.body.appendChild(x);return x;}
var FLY='M0 0C-70 -120 -270 -150 -260 -40C-250 50 -95 65 -25 -40C55 -160 280 -270 760 -460';
var canPath=window.CSS&&CSS.supports&&CSS.supports('offset-path','path("M0 0L1 1")');
function throwPlane(done){
var ta=form.querySelector('textarea'),tr=ta.getBoundingClientRect();
bot.classList.remove('ctc-shy');shy=false;
bot.classList.add('ctc-joy','ctc-wind');
var hb=hr.getBoundingClientRect();
var sheet=el('div','ctc-sheet');sheet.style.left=tr.left+'px';sheet.style.top=tr.top+'px';sheet.style.width=tr.width+'px';sheet.style.height=tr.height+'px';
form.classList.add('ctc-taken');
setTimeout(function(){
hb=hr.getBoundingClientRect();
var tx=hb.left+hb.width/2-20-tr.left,ty=hb.top-14-tr.top,sx=40/tr.width,sy=28/tr.height;
var a=sheet.animate([{transform:'none',borderRadius:'12px'},{transform:'translate('+tx*.55+'px,'+(ty*.55-40)+'px) scale('+(sx*3)+','+(sy*3)+') rotate(-8deg)',borderRadius:'30px',offset:.55},{transform:'translate('+tx+'px,'+ty+'px) scale('+sx+','+sy+') rotate(-20deg)',borderRadius:'40px'}],{duration:620,easing:'cubic-bezier(.5,0,.3,1)',fill:'forwards'});
a.onfinish=function(){
hb=hr.getBoundingClientRect();
var ox=hb.left+hb.width/2,oy=hb.top-4;
sheet.remove();
var plane=el('div','ctc-plane',PLANE);plane.style.left=ox+'px';plane.style.top=oy+'px';
say('Off it goes!',2200);
setTimeout(function(){
bot.classList.remove('ctc-wind');bot.classList.add('ctc-throw','ctc-track');
setTimeout(function(){bot.classList.remove('ctc-throw');},380);
var trail=el('div','ctc-trail','<svg width="1" height="1" style="overflow:visible"><defs><mask id="ctcmk" maskUnits="userSpaceOnUse" x="-2000" y="-2000" width="4000" height="4000"><path d="'+FLY+'" pathLength="1" fill="none" stroke="#fff" stroke-width="6" stroke-dasharray="1 1" stroke-dashoffset="1"><animate attributeName="stroke-dashoffset" from="1" to="0" dur="1.7s" fill="freeze" calcMode="spline" keyTimes="0;1" keySplines=".45 .05 .35 1"/></path></mask></defs><path d="'+FLY+'" fill="none" stroke="currentColor" stroke-width="2" stroke-dasharray="3 7" stroke-linecap="round" mask="url(#ctcmk)" opacity=".55"/></svg>');
trail.style.left=ox+'px';trail.style.top=oy+'px';trail.style.color=getComputedStyle(C).getPropertyValue('--ink');
var fa;
if(canPath){plane.style.offsetPath='path("'+FLY+'")';plane.style.offsetRotate='auto -18deg';fa=plane.animate([{offsetDistance:'0%'},{offsetDistance:'100%'}],{duration:1700,easing:'cubic-bezier(.45,.05,.35,1)',fill:'forwards'});}
else{fa=plane.animate([{transform:'translate(0,0) rotate(-20deg)'},{transform:'translate(-240px,-120px) rotate(-160deg)',offset:.4},{transform:'translate(760px,-460px) rotate(-30deg)'}],{duration:1700,easing:'ease-in-out',fill:'forwards'});}
var t0=performance.now();
(function track(){var pr=plane.getBoundingClientRect();lookAt(pr.left+pr.width/2,pr.top+pr.height/2);if(performance.now()-t0<1750)requestAnimationFrame(track);})();
bot.classList.remove('ctc-joy');
fa.onfinish=function(){plane.remove();trail.animate([{opacity:1},{opacity:0}],{duration:400,fill:'forwards'}).onfinish=function(){trail.remove();};bot.classList.remove('ctc-track');look(0,0);bot.classList.add('ctc-joy');wave();setTimeout(done,700);};
},120);
};
},300);
}
form.addEventListener('submit',function(e){
if(busy)return;
var hp=form.querySelector('[name="_honey"]');if(hp&&hp.value)return;
e.preventDefault();busy=true;
if(reduce||!document.body.animate){HTMLFormElement.prototype.submit.call(form);return;}
throwPlane(function(){HTMLFormElement.prototype.submit.call(form);});
});
window.addEventListener('pageshow',function(e){if(e.persisted){busy=false;form.classList.remove('ctc-taken');bot.classList.remove('ctc-joy','ctc-wind','ctc-throw','ctc-track','ctc-shy');}});
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
