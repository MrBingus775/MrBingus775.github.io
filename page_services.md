---
layout: page
title: Consulting Services
permalink: /services/
path: /services/
order: 2
---

<div class="scroller" id="scroller">
<section id="executive-briefings">

  <h2>Executive Briefings</h2>

  <p class="services-txt">
  Pantheon Insights provides concise executive briefings to equip leaders with a competitive edge to fortify their business operations in the dynamic terrain of geopolitics. Our insights enable clients to deploy proactive strategies for navigating complex global dynamics with confidence and clarity. 
  </p>

  <div class="services-contact">
    <div style="text-align: center;">
      <div><a href="/contact" class="btn btn-lg btn-primary">Request an Executive Briefing</a></div>
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
  <h2>Speaking</h2>

  <p class="services-txt">
  In an increasingly convoluted world, the threshold for understanding unprecedented changes is rising at a commensurate rate to the rapid evolution of modern international affairs. Pantheon Insights founder Dimitri Zabelin’s research has been cited in think tanks and global media publications including BBC News, the World Economic Forum, Reuters, The Diplomat and many others that have translated his work in Asia, Latin America, and Europe.
  </p>

  <div class="services-contact">
    <div style="text-align: center;">
      <a href="/contact" class="btn btn-lg btn-primary">Request a Media Appearance</a>
    </div>
  </div>

  <div class="scroll-caret-parent row">
    <a class="scroll-caret center-image" data-bs-toggle="collapse" role="button">
      <div class="mt-2"/>
      <img src="/assets/icons/caret-down.svg" class="caret-down" alt="caret" width="40" height="40"/>
    </a>
  </div>
</section>


<section id="geo-series-forecasts">
  <h2>Geo-Series Forecasts</h2>

  <p class="services-txt">
  Pantheon Insights offers a unique triad series analyzing the interplay and individual dynamics of geopolitical, geofinancial, and geoeconomic trends in Asia, the Americas, Europe and Africa. As the Rubik’s Cube of 21st-century globalization continues to confound business leaders, Pantheon Insights offers tools to understand trend-defining characteristics of the new global paradigm. 
  </p>

  <div class="services-contact">
    <div style="text-align: center;">
      <a href="/contact" class="btn btn-lg  btn-primary">Request a Geo-Series Theme</a>
    </div>
  </div>

  <div class="scroll-caret-parent row">
    <a class="scroll-caret center-image" data-bs-toggle="collapse" role="button">
      <div class="mt-2"/>
      <img src="/assets/icons/caret-down.svg" class="caret-down" alt="caret" width="40" height="40"/>
    </a>
  </div>
</section>


<section id="thought-leadership">
  <h2>Thought Leadership</h2>

  <p class="services-txt">
  Pantheon Insight partners with clients to produce comprehensive white papers, foster research collaborations, op-eds, and original thought leadership on the intersection of geopolitics, markets, and economies. Our expertise drives informed discussions and empowers our clients to make sound, strategic decisions in a rapidly evolving world.
  </p>

  <div class="services-contact">
    <div style="text-align: center;">
      <a href="/contact" class="btn btn-lg btn-primary">Request Thought Leadership</a>
    </div>
  </div>
</section>
</div>

<div class="container-fluid text-center" style="margin-top: 80px; font-size: 20px;">
  <p>
    <span class="services-nav-link" targetSection="#executive-briefings"><a role="button" class="">Executive Briefings</a></span>
    |
    <span class="services-nav-link" targetSection="#speaking"><a role="button" class="">Speaking</a></span>
    |
    <span class="services-nav-link" targetSection="#geo-series-forecasts"><a role="button" class="">Geo-Series Forecasts</a></span>
    |
    <span class="services-nav-link" targetSection="#thought-leadership"><a role="button" class="">Thought Leadership</a></span>
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