---
layout: page
title: Consulting Services
permalink: /services/
path: /services/
order: 2
description: "Requests for advisory services, speaking engagements, strategic insights, and briefings"
---

<div class="scroller slide-in" id="scroller">
<section id="advisory-services">

  <h2>Advisory Services</h2>

  <p class="services-txt">
  Tailored advisory solutions address the unique challenges posed by shifting geopolitical dynamics. Each consultation offers actionable strategies to mitigate risks and capitalize on emerging opportunities. Designed for adaptability, these services ensure clients remain resilient in a rapidly changing world.
  </p>

  <div class="services-contact">
    <div style="text-align: center;">
      <div><a href="/contact" class="primary-button-lg">Request Advisory Services</a></div>
    </div>
  </div>

  <div class="scroll-caret-parent row">
    <a class="scroll-caret center-image" data-bs-toggle="collapse" role="button">
      <div class="mt-2"/>
      <img src="/assets/icons/caret-down.svg" class="caret-down" alt="caret" width="40" height="40"/>
    </a>
  </div>
</section>


<section id="strategic-insights">
  <h2>Strategic Insights</h2>

  <p class="services-txt">
  Strategic insights provide forward-looking analyses, blending geopolitical expertise with data-driven methodologies. The focus is on identifying trends that shape global markets, impact macroeconomic dynamics, and influence policy decisions. Built for flexibility, these insights enhance maneuverability in a rapidly evolving landscape.
  </p>

  <div class="services-contact">
    <div style="text-align: center;">
      <a href="/contact" class="primary-button-lg">Request Strategic Insights</a>
    </div>
  </div>

  <div class="scroll-caret-parent row">
    <a class="scroll-caret center-image" data-bs-toggle="collapse" role="button">
      <div class="mt-2"/>
      <img src="/assets/icons/caret-down.svg" class="caret-down" alt="caret" width="40" height="40"/>
    </a>
  </div>
</section>


<section id="executive-briefings">
  <h2>Executive briefings</h2>

  <p class="services-txt">
  Executive briefings offer tailored insights into the evolving geopolitical landscape. Each briefing provides actionable strategies to navigate complex global dynamics with confidence and clarity. Designed for adaptability, these services ensure clients remain resilient in a rapidly changing world.
  </p>

  <div class="services-contact">
    <div style="text-align: center;">
      <a href="/contact" class="primary-button-lg">Request an Executive Briefing</a>
    </div>
  </div>

  <div class="scroll-caret-parent row">
    <a class="scroll-caret center-image" data-bs-toggle="collapse" role="button">
      <div class="mt-2"/>
      <img src="/assets/icons/caret-down.svg" class="caret-down" alt="caret" width="40" height="40"/>
    </a>
  </div>
</section>


<section id="speaking">
  <h2>Speaking engagements</h2>

  <p class="services-txt">
  Speaking engagements explore the geopolitical dynamics shaping today’s world, offering a balanced perspective on emerging trends. Delivered with clarity, they provide actionable insights to help audiences navigate complex challenges. Each session is designed to inspire strategic thinking and foster informed decision-making.
  </p>

  <div class="services-contact">
    <div style="text-align: center;">
      <a href="/contact" class="primary-button-lg">Request Speaking Engagements</a>
    </div>
  </div>
</section>
</div>

<div class="container-fluid text-center slide-in" style="margin-top: 80px; font-size: 20px;">
  <p>
    <span class="services-nav-link" targetSection="#advisory-services"><a role="button" class="">Advisory Services</a></span>
    |
    <span class="services-nav-link" targetSection="#strategic-insights"><a role="button" class="">Strategic Insights</a></span>
    |
    <span class="services-nav-link" targetSection="#executive-briefings"><a role="button" class="">Executive Briefings</a></span>
    |
    <span class="services-nav-link" targetSection="#speaking"><a role="button" class="">Speaking Engagements</a></span>
  </p>
</div>


<script>
  // Click handler on all elements with class 'scroll-caret'
  $('.scroll-caret-parent').click(function() {
    console.log("scroll-caret clicked");

    const container = document.getElementById('scroller');

    // Get the parent of the clicked element
    const parent = this.parentElement;

    // Get the element following the parent
    const nextSection = parent.nextElementSibling;

    // Scroll to the next section, making note that all sections are wrapped on a scroll-snap boundary
    // This is to prevent the scroll from stopping in the middle of a section
    container.scrollTo({
      top: nextSection.offsetTop,
      behavior: 'smooth'
    });
  });

  // Add a click handler to all elements with class 'services-nav-link'
  $('.services-nav-link').click(function() {
    console.log("services-nav-link clicked");

    const container = document.getElementById('scroller');

    // Get the id of the section to scroll to
    const sectionId = this.getAttribute('targetSection');

    console.log("sectionId: " + sectionId)

    // Get the section to scroll to
    const section = document.querySelector(sectionId);

    // Scroll to the section, making note that all sections are wrapped on a scroll-snap boundary
    // This is to prevent the scroll from stopping in the middle of a section
    container.scrollTo({
      top: section.offsetTop,
      behavior: 'smooth'
    });
  });


</script>