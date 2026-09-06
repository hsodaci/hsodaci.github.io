---
title: Contact
permalink: /contact/
layout: page
excerpt: Get in touch with Hande Sodacı.
comments: false
---

Have a question, an opportunity, or just want to say hi? Send a message below and it'll land directly in my inbox.

<form action="https://formsubmit.co/{{ site.author.email }}" method="POST" class="contact-form">
  <!-- Plain-text email notification, no fancy template -->
  <input type="hidden" name="_subject" value="New message from hsodaci.github.io">
  <!-- Honeypot field to cut down on bot spam -->
  <input type="text" name="_honey" style="display:none">
  <!-- Skip FormSubmit's captcha interstitial -->
  <input type="hidden" name="_captcha" value="false">
  <!-- Send visitors back here with a confirmation message -->
  <input type="hidden" name="_next" value="{{ site.url }}/contact/?sent=true">

  <label for="name">Name</label>
  <input type="text" id="name" name="name" required>

  <label for="email">Email</label>
  <input type="email" id="email" name="email" required>

  <label for="message">Message</label>
  <textarea id="message" name="message" rows="6" required></textarea>

  <button type="submit">Send</button>
</form>

<p id="contact-sent" class="contact-sent" hidden>Thanks — your message is on its way!</p>

<script>
  if (window.location.search.includes('sent=true')) {
    document.getElementById('contact-sent').hidden = false;
  }
</script>

<!--
  This form uses FormSubmit (https://formsubmit.co) to relay submissions to
  {{ site.author.email }} without needing a backend server. The FIRST
  submission after this page goes live will trigger a one-time confirmation
  email from FormSubmit to {{ site.author.email }} — you must click the
  activation link in that email before the form will actually deliver
  messages.
-->
