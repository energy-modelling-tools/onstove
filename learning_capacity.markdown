---
theme: jekyll-theme-primer
layout: sub-page
title: OnStove
permalink: /learning_capacity/
---

<section class="bg-gray-light py-5 fade-in-center">
  <div class="container-lg p-responsive">

    <!-- Title -->
    <div class="text-center fade-in-center">
      <h2 class="alt-h2 mb-4">Learning & Capacity Building</h2>
    </div>

    <!-- E-Learning Section -->
    <div class="mt-3 animate-in">
      <h3 class="alt-h3 mt-3" style="font-size: 1.25rem;">📘 Open University Course on Geospatial Clean Cooking Access Modelling using OnStove</h3>
      <p class="animate-in" style="font-size: 0.95rem;">
        In this course, you will learn about geospatial clean cooking modelling and how to build your own clean cooking transition scenarios using spatial data. 
        You will be introduced to <strong>OnStove</strong>—an open-source spatial clean cooking tool that identifies the best cooking solutions across any given area based on their costs and benefits. 
        You will learn how to create your own spatial repository, modify spatial datasets, calculate the net benefits of different cooking solutions, and visualize and present your results.
      </p>
      <p class="animate-in">
        <a href="https://www.open.edu/openlearncreate/course/view.php?id=11724" target="_blank" class="btn btn-outline-primary sky-blue-accent d-block d-sm-inline-block px-1 px-md-3" style="border-color: #3490dc; color: #3490dc;">
          Access the Course →
        </a>
      </p>
    </div>

    <!-- Interface / Kits (Future Features Placeholder) -->
    <div class="mt-5 animate-in">
      <h3 class="alt-h3 mt-3" style="font-size: 1.25rem;">📦 Upcoming Resources</h3>
      <ul class="animate-in">
        <li><strong>Starter Data Kits</strong> – Coming soon</li>
        <li><strong>Flatpack Program</strong> – Coming soon</li>
        <li><strong>Energy Modelling Community (YouTube Playlist)</strong> – Coming soon</li>
      </ul>
    </div>

    <!-- EMP Section -->
    <div class="mt-5 animate-in">
      <h3 class="alt-h3 mt-3" style="font-size: 1.25rem;">🌍 Energy Modelling Platforms (EMPs)</h3>
      <p class="animate-in" style="font-size: 0.95rem;">
        OnStove has been part of the Energy Modelling Platform – Global (EMP-G) series since 2023, where it is taught as a spatial clean cooking modelling component. 
        Through EMPs, analysts and policymakers from around the world gain hands-on experience developing clean cooking transition scenarios and sharing results through Zenodo and conference presentations.
      </p>
    </div>

    <!-- EMP Events Section -->
    <div class="container-lg p-responsive py-4 py-md-6 my-lg-6 animate-in">
      <h3 class="alt-h3 text-center mb-3 animate-in" style="font-size: 1.25rem;">🌍 Explore EMP Events</h3>

      <div class="clearfix gutter-spacious">
        {% for event in site.data.learning_events.events %}
        <div class="col-md-4 float-left animate-in mb-4">
          <h3 class="alt-h3 mb-3">{{ event.title }}</h3>
          <p class="text-gray">{{ event.description }}</p>
          <details class="animate-in">
            <summary class="btn btn-sm btn-outline toggle-arrow">Show Outputs</summary>
            <ul class="mt-2">
              {% for output in event.outputs %}
              <li class="animate-in">
                {{ output.flag }} <strong>{{ output.country }}</strong>: 
                <a href="{{ output.url }}" target="_blank">{{ output.title }}</a>
              </li>
              {% endfor %}
            </ul>
          </details>
        </div>
        {% endfor %}
      </div>
    </div>

    <!-- Other Related Events -->
    <div class="container-lg p-responsive py-4 py-md-6 my-lg-6 animate-in">
      <h3 class="alt-h3 text-center mb-3 animate-in" style="font-size: 1.25rem;">🔎 Other Related Events</h3>

      <div class="clearfix gutter-spacious">
        {% for other in site.data.learning_events.other_events %}
        <div class="col-md-12 animate-in mb-4">
          <h4 class="alt-h4 mb-2">{{ other.title }}</h4>
          <p class="text-gray">{{ other.description }}</p>
          <p class="animate-in">
            <a href="{{ other.url }}" target="_blank" class="btn btn-outline-primary sky-blue-accent" style="border-color: #3490dc; color: #3490dc;">
              Learn more →
            </a>
          </p>
        </div>
        {% endfor %}
      </div>
    </div>

  </div>
</section>

<style>
/* Fade-in animation for main title */
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

/* Animate-in effects for all elements */
.animate-in {
  opacity: 0;
  transform: translateY(30px);
  animation: animateIn 0.8s ease-out forwards;
  animation-delay: var(--animation-delay, 0s);
}

/* Staggered animation delays */
.animate-in:nth-child(1) { --animation-delay: 0.1s; }
.animate-in:nth-child(2) { --animation-delay: 0.2s; }
.animate-in:nth-child(3) { --animation-delay: 0.3s; }
.animate-in:nth-child(4) { --animation-delay: 0.4s; }
.animate-in:nth-child(5) { --animation-delay: 0.5s; }
.animate-in:nth-child(6) { --animation-delay: 0.6s; }
.animate-in:nth-child(7) { --animation-delay: 0.7s; }
.animate-in:nth-child(8) { --animation-delay: 0.8s; }
.animate-in:nth-child(9) { --animation-delay: 0.9s; }
.animate-in:nth-child(10) { --animation-delay: 1.0s; }

/* Column animations with staggered delays for 3-column layout */
.col-md-4.float-left.animate-in:nth-child(1) { animation-delay: 0.1s; }
.col-md-4.float-left.animate-in:nth-child(2) { animation-delay: 0.2s; }
.col-md-4.float-left.animate-in:nth-child(3) { animation-delay: 0.3s; }

/* Column hover effects */
.col-md-4.float-left {
  transition: all 0.3s ease;
  display: flex;
  flex-direction: column;
  height: 100%;
}

.col-md-4.float-left:hover {
  transform: translateY(-4px);
}

/* Standardize column height and content distribution */
.col-md-4.float-left > h3 {
  flex-shrink: 0;
  min-height: 5rem;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  margin-bottom: 1rem;
  line-height: 1.3;
}

.col-md-4.float-left > p:first-of-type {
  flex-shrink: 0;
  text-align: center;
  margin-bottom: 1rem;
}

/* Standardized image container */
.col-md-4 img {
  width: 100%;
  height: 220px;
  object-fit: cover;
  object-position: center;
  border-radius: 8px;
  transition: transform 0.3s ease;
}

.col-md-4 img:hover {
  transform: scale(1.02);
}

/* Text content area - flexible height */
.col-md-4.float-left > p.text-gray {
  flex: 1;
  margin-bottom: 1.5rem;
  line-height: 1.5;
}

/* Details section at bottom - aligned */
.col-md-4.float-left > details {
  margin-top: auto;
  align-self: flex-start;
}

/* Button alignment */
.col-md-4.float-left > details > summary {
  margin: 0;
}

/* List item animations */
li.animate-in:nth-child(1) { animation-delay: 0.1s; }
li.animate-in:nth-child(2) { animation-delay: 0.2s; }
li.animate-in:nth-child(3) { animation-delay: 0.3s; }
li.animate-in:nth-child(4) { animation-delay: 0.4s; }
li.animate-in:nth-child(5) { animation-delay: 0.5s; }
li.animate-in:nth-child(6) { animation-delay: 0.6s; }
li.animate-in:nth-child(7) { animation-delay: 0.7s; }
li.animate-in:nth-child(8) { animation-delay: 0.8s; }
li.animate-in:nth-child(9) { animation-delay: 0.9s; }

@keyframes animateIn {
  from {
    opacity: 0;
    transform: translateY(30px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Hover effects for interactive elements */
.animate-in:hover {
  transform: translateY(-2px);
  transition: transform 0.3s ease;
}

/* Enhanced container animations */
.container .animate-in {
  animation-delay: 0.3s;
}

/* Button hover animations */
.btn.animate-in:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
  transition: all 0.3s ease;
}

/* Image animations */
img.animate-in:hover {
  transform: scale(1.05);
  transition: transform 0.3s ease;
}

.toggle-arrow::after {
  content: '↓';
  display: inline-block;
  margin-left: 6px;
  transition: transform 0.3s ease;
}
details[open] .toggle-arrow::after {
  transform: rotate(180deg);
}
</style>