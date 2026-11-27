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
</style>
<div class="ctc">
<h1 class="ctc-h1">Contact<span>.</span></h1>
<p class="ctc-lead">Have a question, an opportunity, or just want to say hi? Send a message below and I will get back to you as soon as possible.</p>
<div class="ctc-card">
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
<p id="contact-sent-title" class="ctc-mt">Message received</p>
<button type="button" id="contact-sent-close" class="ctc-close">Close</button>
</div>
</div>
</div>
<script>
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
