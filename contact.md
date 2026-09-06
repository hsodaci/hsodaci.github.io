---
title: Contact
permalink: /contact/
layout: page
excerpt: Get in touch with Hande Sodacı.
comments: false
---

<p class="contact-lead">Have a question, an opportunity, or just want to say hi? Send a message below and I will get back to you as soon as possible.</p>

<div class="contact-card">
  <form action="https://formsubmit.co/{{ site.author.email }}" method="POST" class="contact-form">
    <!-- Plain-text email notification, no fancy template -->
    <input type="hidden" name="_subject" value="New message from hsodaci.github.io">
    <!-- Honeypot field to cut down on bot spam -->
    <input type="text" name="_honey" style="display:none">
    <!-- Skip FormSubmit's captcha interstitial -->
    <input type="hidden" name="_captcha" value="false">
    <!-- Send visitors back here with a confirmation message -->
    <input type="hidden" name="_next" value="{{ site.url }}/contact/?sent=true">

    <div class="field">
      <label for="name">Your name</label>
      <input type="text" id="name" name="name" placeholder="Jane Doe" required>
    </div>

    <div class="field">
      <label for="email">Email address</label>
      <input type="email" id="email" name="email" placeholder="jane@example.com" required>
    </div>

    <div class="field">
      <label for="message">Message</label>
      <textarea id="message" name="message" rows="6" placeholder="What can I help with?" required></textarea>
    </div>

    <button type="submit">Send message</button>
  </form>

</div>

<div id="contact-sent-overlay" class="contact-modal-overlay" hidden>
  <div class="contact-modal" role="dialog" aria-modal="true" aria-labelledby="contact-sent-title">
    <p id="contact-sent-title" class="contact-modal-title">Message received</p>
    <button type="button" id="contact-sent-close" class="contact-modal-close">Close</button>
  </div>
</div>

<script>
  (function () {
    if (!window.location.search.includes('sent=true')) return;

    var overlay = document.getElementById('contact-sent-overlay');
    var closeBtn = document.getElementById('contact-sent-close');

    function closeModal() {
      overlay.hidden = true;
      var url = new URL(window.location.href);
      url.searchParams.delete('sent');
      window.history.replaceState({}, '', url);
    }

    overlay.hidden = false;
    closeBtn.addEventListener('click', closeModal);
    overlay.addEventListener('click', function (e) {
      if (e.target === overlay) closeModal();
    });
    document.addEventListener('keydown', function (e) {
      if (e.key === 'Escape') closeModal();
    });
  })();
</script>

<!--
  This form uses FormSubmit (https://formsubmit.co) to relay submissions to
  {{ site.author.email }} without needing a backend server. The FIRST
  submission after this page goes live will trigger a one-time confirmation
  email from FormSubmit to {{ site.author.email }} — you must click the
  activation link in that email before the form will actually deliver
  messages.
-->
