---
title: contact details
layout: default
type: contact
permalink: /contact
---

<div markdown="1" class="contact">

## Contact

[<i class="fa fa-envelope"></i> Appiah.harrison@yahoo.com](mailto:Appiah.harrison@yahoo.com)

---

## Send me a message

<form action="https://api.web3forms.com/submit" method="POST" class="contact-form">

  <!-- Replace with your Web3Forms access key -->
  <input type="hidden" name="access_key" value="01621979-a3fe-4a30-8804-76e20a8f7dc9">

  <!-- Honeypot spam protection -->
  <input type="checkbox" name="botcheck" style="display: none;">

  <label>
    Your Name*
    <input type="text" name="name" required>
  </label>

  <label>
    Your Email*
    <input type="email" name="email" required>
  </label>

  <label>
    Message*
    <textarea name="message" rows="4" required></textarea>
  </label>

  <!-- Optional subject line -->
  <input type="hidden" name="subject" value="New message from ngtanikella.github.io">

  <button type="submit">Send Message</button>
  <input type="hidden" name="redirect" value="{{site.url}}{{site.baseurl}}/thank-you/">
</form>

<style>
.contact-form{
  max-width: 720px;
  display: grid;
  gap: 0.9rem;
  margin-top: 1rem;
}

.contact-form label{
  display: grid;
  gap: 0.4rem;
  font-weight: 600;
}

.contact-form input,
.contact-form textarea{
  width: 100%;
  padding: 0.7rem 0.8rem;
  border: 1px solid rgba(0,0,0,0.18);
  border-radius: 12px;
  font: inherit;
}

.contact-form button{
  width: fit-content;
  padding: 0.65rem 1rem;
  border-radius: 12px;
  border: 1px solid rgba(0,0,0,0.2);
  cursor: pointer;
  font-weight: 700;
}
</style>

---

[<img src="{{site.url}}{{site.baseurl}}/docs/cv/Logos/Google_Scholar_logo.svg.png" alt="Google Scholar" class="inline-logo"> Google Scholar]({{ site.google_scholar_url }}){:target="_blank"}


[<img src="{{site.url}}{{site.baseurl}}/docs/cv/Logos/ORCID.png" alt="ORCID" class="inline-logo"> ORCID]([https://orcid.org/0000-0003-1678-1932](https://orcid.org/0000-0002-1101-7225){:target="_blank"}

[<img src="{{site.url}}{{site.baseurl}}/docs/cv/Logos/Academia.jpeg" alt="Academia" class="inline-logo"> Academia](https://https://uidaho.academia.edu/HarrisonAppiah){:target="_blank"}

</div>
