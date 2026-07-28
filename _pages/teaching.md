---
layout: page
permalink: /teaching/
title: Teaching
description:
nav: true
nav_order: 2
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
  /* Smaller headshot, forced into a true circle regardless of the source image shape. */
  .profile {
    max-width: 190px;
  }
  .profile.float-right {
    margin-left: 2rem;
  }
  .profile img {
    aspect-ratio: 1 / 1;
    object-fit: cover;
    border-radius: 50%;
  }
  /* On small screens, stack the photo block above the text instead of floating beside it. */
  @media (max-width: 575.98px) {
    .profile.float-right {
      float: none;
      margin: 0 auto 1.5rem;
    }
  }
  /* Role / institution lines + social links: one shared block, sized to its
     widest line and centered as a unit under the photo, with everything left-
     aligned inside so the icons all line up on the same left edge. */
  .profile-info {
    margin-top: 0.75rem;
    width: fit-content;
    margin-left: auto;
    margin-right: auto;
    text-align: left;
    font-size: 0.8rem;
  }
  .profile-info > div {
    margin-bottom: 0.25rem;
  }
  .profile-info a {
    color: var(--global-text-color);
  }
  .profile-info a:hover {
    color: var(--global-theme-color);
  }
  .profile-info i {
    margin-right: 0.4rem;
    width: 1em;
    text-align: center;
  }
  .profile-info .meta-line i {
    color: var(--global-text-color-light);
  }
  /* Bordered text column: shrinks to avoid running under the floated photo. */
  .content-border {
    display: flow-root;
    border: 1px solid var(--global-divider-color);
    border-radius: 8px;
    padding: 1.25rem 1.5rem;
    text-align: justify;
  }
  .course {
    margin-bottom: 2.5rem;
  }
  /* Course titles stay left-aligned (justify looks odd once they wrap on mobile). */
  .course h2 {
    margin-bottom: 0.2rem;
    text-align: left;
  }
  .course .course-meta {
    color: var(--global-text-color-light);
    margin-bottom: 0.8rem;
  }
  .course .resource-list {
    list-style: none;
    padding-left: 0;
  }
  .course .resource-list li {
    margin-bottom: 0.4rem;
  }
  /* Student testimonials: smaller and grey. */
  .course blockquote {
    font-size: 0.85rem;
    color: var(--global-text-color-light);
  }
</style>

<script>
  (function () {
    var links = document.querySelectorAll("a.nav-link");
    var cvLink = null;
    for (var i = 0; i < links.length; i++) {
      var href = links[i].getAttribute("href") || "";
      if (/\/cv\/?($|[?#])/i.test(href)) {
        cvLink = links[i];
        break;
      }
    }
    if (!cvLink) return;
    cvLink.addEventListener("click", function (e) {
      e.preventDefault();
      window.open("/assets/pdf/Ruby (Ruishan) Zhang Curriculum Vitae.pdf", "_blank", "noopener");
    });
  })();
</script>

<div class="profile float-right">
  {% include figure.liquid loading="eager" path="assets/img/headshot1_crop.jpg" class="img-fluid z-depth-1 rounded-circle" alt="Ruby Zhang" %}
  <div class="profile-info">
    <div class="meta-line">PhD Candidate in Economics</div>
    <div class="meta-line"><i class="fa-solid fa-landmark"></i>Harvard University</div>
    <div><a href="mailto:{{ site.data.socials.email }}"><i class="fa-solid fa-envelope"></i>Email</a></div>
    <div>
      <a
        href="https://scholar.google.com/citations?user={{ site.data.socials.scholar_userid }}&hl=en"
        target="_blank"
        rel="noopener"
      >
        <i class="fa-solid fa-graduation-cap"></i>Google Scholar
      </a>
    </div>
    <div>
      <a href="https://www.linkedin.com/in/{{ site.data.socials.linkedin_username }}" target="_blank" rel="noopener">
        <i class="fa-brands fa-linkedin"></i>LinkedIn
      </a>
    </div>
  </div>
</div>

<div class="content-border" markdown="1">

I am grateful to have taught excellent students and courses during my time as a graduate student. I was a teaching fellow for _ECON 1640: Industrial Organization_ (undergraduate) and co-created a computational PhD course _ECON 2003: Computing for Economists_ with [Toren Fronsdal](https://www.linkedin.com/in/fronsdal) and [Jesse Shapiro](https://shapiro.scholars.harvard.edu/).

<div class="course" markdown="0">
  <h2>ECON 2003: Computing for Economists</h2>
  <div class="course-meta">Summer 2024 · Summer 2025</div>
  <p>The course consists of twelve modules and introduces concepts in software engineering and scientific computing that are essential for modern economics research. We created lecture slides and recorded videos which students watched in advance of class sessions. Class sessions were then devoted to supervised group work on coding exercises (which we also designed).</p>

  <p><strong>Lecture Slides</strong></p>
  <ul class="resource-list">
    <li><a href="/assets/pdf/Software_Engineering_and_Version_Control.pdf" target="_blank" rel="noopener">Lecture 1 — Software Engineering and Version Control</a></li>
    <li><a href="/assets/pdf/Data_Wrangling.pdf" target="_blank" rel="noopener">Lecture 2 — Data Wrangling</a></li>
    <li><a href="/assets/pdf/Intro_to_Unix_and_the_Command_Line.pdf" target="_blank" rel="noopener">Lecture 3 — Introduction to Unix and the Command Line</a></li>
    <li><a href="/assets/pdf/Nonlinear_Equation_Solving_and_Derivative-Based_Optimization.pdf" target="_blank" rel="noopener">Lecture 4 — Nonlinear Equation Solving and Derivative-Based Optimization</a></li>
    <li><a href="/assets/pdf/Derivative_Free_and_Constrained_Optimization.pdf" target="_blank" rel="noopener">Lecture 5 — Derivative-Free and Constrained Optimization</a></li>
    <li><a href="/assets/pdf/Numerical_Differentiation_and_Integration.pdf" target="_blank" rel="noopener">Lecture 6 — Numerical Differentiation and Integration</a></li>
    <li><a href="/assets/pdf/Parallelization_and_Big_Data.pdf" target="_blank" rel="noopener">Lecture 7 — Parallelization and Big Data</a></li>
    <li><a href="/assets/pdf/Numerical_Simulation.pdf" target="_blank" rel="noopener">Lecture 8 — Numerical Simulation and Monte Carlo Methods</a></li>
    <li><a href="/assets/pdf/Introduction_to_Algorithms_and_Combinatorial_Optimization.pdf" target="_blank" rel="noopener">Lecture 9 — Introduction to Algorithms and Combinatorial Optimization</a></li>
    <li><a href="/assets/pdf/Dynamic_Programming.pdf" target="_blank" rel="noopener">Lecture 10 — Dynamic Programming</a></li>
    <li><a href="/assets/pdf/Machine_Learning_Methods.pdf" target="_blank" rel="noopener">Lecture 11 — Machine Learning Methods</a></li>
    <li><a href="/assets/pdf/Bandit_Problems_and_Reinforcement_Learning.pdf" target="_blank" rel="noopener">Lecture 12 — Bandit Problems and Reinforcement Learning</a></li>
  </ul>
</div>

<div class="course" markdown="0">
  <h2>ECON 1640: Industrial Organization</h2>
  <div class="course-meta">Fall 2024 · Fall 2025</div>
  <p>As a teaching fellow, I created section materials and held office hours to review the core concepts of firms competing in markets with imperfect competition.</p>

  <p><strong>Selected Teaching Evaluations</strong></p>

  <blockquote>
"Ruby might be the best economics section leader I have ever had [...] I have taken many FOCs in my undergrad degree and solved many different micro problems, but I still feel like I walked away with a better micro foundation from this course, in no small part because of Ruby's sections [...] She cares a lot for her students and this is abundantly evident to how she approaches teaching [...] She's such a kind, wonderful educator that it's hard to not be excited to learn economics during her section. I am so excited for whatever university gets to have Ruby on their faculty!"
  </blockquote>

  <blockquote>
Ruby was seriously a great teaching fellow for this course. She [...] held great enthusiasm for the material and her students. I found the sections to be helpful in enforcing the lecture material, being able to ask questions there as needed.
  </blockquote>

  <blockquote>
"Ruby was an AMAZING TF and was incredibly available to help discuss course materials when I needed. She explains things super digestibly, and knows her stuff very well."
  </blockquote>

  <blockquote>
"Ruby is an excellent teaching fellow. She is very responsive to emails and questions in office hours and is good at breaking down the complicated concepts introduced in lecture. Her section notes are concise and help to reinforce what has been taught through the lecture."
  </blockquote>

   <blockquote>
"Very knowledgeable and very good at explaining the assigned topics – both in section and office hours. Facilitated relevant discussions during section and available and helpful during office hours. Excellent section leader!"
  </blockquote>
</div>

</div>
