---
theme: jekyll-theme-primer
layout: sub-page
title: OnStove
permalink: /about/
---

<section class="bg-gray-light container-lg p-responsive py-4 py-md-6 my-lg-6 fade-in-center">
  <div class="text-center fade-in-center">
    <h2 class="alt-h3 mb-4">About OnStove</h2>
    <div class="container-lg p-responsive py-4 py-md-6">
      <div class="col-md-12 animate-out mb-2">
        <p class="alt-lead text-gray text-justify-between col-md-15 mx-auto">
          <strong>OnStove</strong> is an open-source spatial cost–benefit model developed to identify the most cost-effective and socially beneficial cooking solutions. 
          It evaluates multiple cooking technologies and fuels, incorporating health, environmental, and time-saving benefits alongside economic and technical costs. 
          The tool provides high-resolution spatial outputs that support decision-making for clean cooking transitions in low- and middle-income countries. 
          It can be used both as a standalone geospatial model and as a complementary tool alongside energy system models such as OSeMOSYS and MESSAGE. 
        </p>
      </div>

      <h2 class="aboutpage-subtitle text-left mb-3 mt-lg-6" id="what-does-it-do">What does it aim to do?</h2>
      <div class="col-md-12 animate-out mb-2">
        <p class="alt-lead text-gray text-justify-between col-md-15 mx-auto">
          OnStove quantifies and maps the relative costs and benefits of different cooking technologies—such as LPG, electricity, biogas, and improved biomass—across regions. 
          By accounting for spatially explicit data such as fuel availability, household distribution, and accessibility, the model identifies where interventions can generate 
          the greatest social and environmental returns. This allows planners and policymakers to prioritise clean cooking investments, design context-specific strategies, 
          and evaluate trade-offs between affordability, emissions, and health outcomes.
        </p>
      </div>

      <h2 class="aboutpage-subtitle text-left mb-3 mt-lg-6" id="who-uses-it">Who uses it?</h2>
      <div class="col-md-12 animate-out mb-2">
        <p class="alt-lead text-gray text-justify-between col-md-15 mx-auto">
          The tool is used by governments, research institutions, and development organisations to design and evaluate clean cooking programmes. 
          It supports applications at national, regional, and global scales and provides open access to methodologies, data, and results to encourage collaboration and transparency in the clean cooking sector.
        </p>
      </div>

      <h2 class="aboutpage-subtitle text-left mb-3 mt-lg-6" id="how-to-get-started">How can you get started?</h2>
      <div class="col-md-12 animate-out mb-2">
        <p class="alt-lead text-gray text-justify-between col-md-15 mx-auto">
          The <strong>OnStove documentation</strong> is available on ReadTheDocs and provides a complete guide for installation, data preparation, and running analyses. 
          It also describes the model’s Python functions and workflows for creating national or regional cost–benefit maps for clean cooking solutions.
        </p>
      </div>
    </div>
  </div>

  <!-- Icon Links -->
  <div class="icon-links-section">
    <div class="icon-links-wrapper">

      <!-- GitHub Repository -->
      <div class="icon-link-item">
        <a href="https://github.com/OnStove/onstove" target="_blank">
          <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" width="80" height="80" alt="GitHub" />
          <h3 class="aboutpage-subtitle text-primary">GitHub Repository</h3>
        </a>
      </div>

      <!-- Model Documentation -->
      <div class="icon-link-item">
        <a href="https://onstove.readthedocs.io/en/latest/" target="_blank">
          <img src="/assets/img/Rtdicon.png" width="80" height="80" alt="ReadTheDocs icon" />
          <h3 class="aboutpage-subtitle text-primary">Model Documentation</h3>
        </a>
      </div>

    </div>
  </div>
</section>
  

<style>
.fade-in-center {
  opacity: 0;
  transform: translateY(20px);
  animation: fadeInUp 1s ease forwards;
}
@keyframes fadeInUp {
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
.alt-h3 {
  font-size: 1.15rem;
}
@media (min-width: 768px) {
  .row.justify-content-center > .col-md-4 {
    margin-bottom: 2rem;
  }
}
</style>

