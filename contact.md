---
layout:     page
permalink:  /contact/
style-id:   contact-page
title:      Let's Talk
---

If you're interested in hiring me for engineering, consulting, writing, or editing, shoot me an email at [{{ site.email }}]( mailto:{{ site.email }} ), or just fill out the form below.

<form id="contact-form" action="https://formspree.io/{{ site.email }}" method="POST">
  <div class="form-group">
    <input  type="text"
            name="name"
            placeholder="Your Name"
            class="form-control"
            tabindex="10">
  </div>
  <div class="form-group">
    <input  type="email"
            name="_replyto"
            placeholder="Your Email Address"
            class="form-control"
            tabindex="10">
  </div>
  <div class="form-group">
    <textarea name="message"  
              placeholder="Type your message here."
              class="form-control"
              tabindex="10"></textarea>
  </div>
  
  <input type="submit" value="Send" class="btn btn-primary col-xs-12 col-sm-6" tabindex="10">
</form>