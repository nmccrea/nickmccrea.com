---
layout:     page
html_title: Contact Me
permalink:  /contact/
style-id:   contact-page
title:      Talk to Me
---

Have some reason you want to talk to me? The internet, in its bounty, has provided a place just for that. Feel free to fill out the form below (or you can shoot me an email at [{{ site.email }}]( mailto:{{ site.email }} )).

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

  <input type="submit" value="Send" class="btn btn-primary" tabindex="10">
</form>
