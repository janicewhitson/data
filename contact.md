---
title: Contact
permalink: /contact/
---

<form action="https://formspree.io/f/YOUR-FORM-ID" method="POST">
  <p>
    <label for="name">Name</label><br>
    <input type="text" id="name" name="name" required style="width:100%; padding:0.5rem; margin-top:0.25rem;">
  </p>
  <p>
    <label for="email">Email</label><br>
    <input type="email" id="email" name="_replyto" required style="width:100%; padding:0.5rem; margin-top:0.25rem;">
  </p>
  <p>
    <label for="message">Message</label><br>
    <textarea id="message" name="message" rows="6" required style="width:100%; padding:0.5rem; margin-top:0.25rem;"></textarea>
  </p>
  <button type="submit" style="padding:0.6rem 1.25rem; background:var(--color-accent); color:#fff; border:none; border-radius:6px; cursor:pointer;">Send</button>
</form>
