---
layout: about
title: About
permalink: /
subtitle:
nav: false # the navbar auto-adds the homepage as the "about" tab; nav:true would duplicate it
nav_order: 1

# NOTE: the photo + social icons are built by hand in the page body below so the
# icons can sit directly under the photo. That is why there is no `profile:` block
# here and `social` is set to false (the layout would otherwise put icons at the
# very bottom of the page).
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false # icons are rendered manually under the photo below

announcements:
  enabled: false # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

<style>
  /* Site accent / link color (overrides the theme's default magenta). */
  :root {
    --global-theme-color: #0076df;
    --global-hover-color: #0076df;
  }
  html[data-theme="dark"] {
    --global-theme-color: #58a6ff;
    --global-hover-color: #58a6ff;
  }
  /* Force the headshot into a true circle regardless of the source image shape. */
  .profile img {
    aspect-ratio: 1 / 1;
    object-fit: cover;
    border-radius: 50%;
  }
  /* Social icons: smaller and centered directly beneath the photo. */
  .profile .social {
    margin-top: 0.6rem;
    text-align: center;
  }
  .profile .social .contact-icons {
    font-size: 1.7rem;
  }
  .profile .social .contact-icons a {
    margin: 0 0.3rem;
  }
</style>

<div class="profile float-right">
  {% include figure.liquid loading="eager" path="assets/img/headshot1_crop.jpg" class="img-fluid z-depth-1 rounded-circle" alt="Ruby Zhang" %}
  <div class="social">
    <div class="contact-icons">{% social_links %}</div>
  </div>
</div>

<div style="text-align: justify;" markdown="1">

Welcome to my website! I am a PhD candidate in Economics at Harvard University. I study innovation and industrial organization, with a focus on digitization and AI.

**I am on the 2026-2027 job market.**

I am a graduate affiliate of the [Institute for Quantitative Social Science](https://www.iq.harvard.edu/). Prior to the PhD, I worked as a Pre-Doctoral Fellow at [Opportunity Insights](https://opportunityinsights.org/) and graduated from the University of Chicago in 2019.

You can reach me at [rzhang15@g.harvard.edu](mailto:rzhang15@g.harvard.edu).

</div>
