---
theme: jekyll-theme-primer
layout: sub-page
title: OnStove
permalink: /applications/
---

<section class="bg-gray-light container-lg p-responsive py-4 py-md-6 my-lg-6 fade-in-center">
  <div class="text-center fade-in-center">
    <h2 class="alt-h2 mb-4">OnStove Applications</h2>
  </div>

  <div class="applications-content text-left">
    <p class="lead mb-4">
      <em>‘OnStove’</em> is a fundamental building block for a wide range of applications across government, industry, and academia. 
      Several examples include:
    </p>

    <div class="applications-grid">

      <!-- Governments -->
      <div class="application-category">
        <h3 class="category-title">Governments</h3>
        <p>
          OnStove has supported clean cooking transition plans in Nepal and Kenya as part of collaborations with the Clean Cooking Alliance, 
          the World Resources Institute, the Kenyan Energy Ministry, and Nepal’s Alternative Energy Promotion Center (AEPC).
        </p>
      </div>

      <!-- Industry and Think Tanks -->
      <div class="application-category">
        <h3 class="category-title">Industry and Think Tanks</h3>
        <p>
          OnStove has been used by international organizations to inform clean cooking access strategies:
        </p>
        <ul class="application-list">
          <li>
            <a href="https://www.iea.org/reports/a-vision-for-clean-cooking-access-for-all" target="_blank">
              OnStove informed clean cooking adoption scenarios in the IEA’s 2023 special report 
              <em>“A Vision for Clean Cooking Access for All.”</em>
            </a>
          </li>
          <li>
            <a href="https://www.wri.org/update/energy-access-explorer-open-software-enabling-access-clean-cooking-nepal" target="_blank">
              OnStove results were integrated into Nepal’s Energy Access Explorer by the World Resources Institute (WRI), 
              KTH Royal Institute of Technology, and AEPC. 
              This effort helped to capture key geospatial parameters of unserved and underserved populations across the country 
              and supported better planning of clean cooking transitions.
            </a>
          </li>
          <li>
            <a href="https://www.wri.org/update/leveraging-energy-access-explorer-advance-kenyas-clean-cooking-agenda" target="_blank">
              OnStove results were integrated into Kenya’s Energy Access Explorer by WRI, KTH Royal Institute of Technology, 
              and the Ministry of Energy. 
              It supported scenario analysis to identify least-cost clean cooking options across counties and 
              helped inform national investment priorities for clean cooking access.
            </a>
          </li>
        </ul>
      </div>

      <!-- Academia -->
      <div class="application-category">
        <h3 class="category-title">Academia</h3>
        <ul class="application-list">
          <li>
            <a href="https://doi.org/10.1038/s41893-022-01039-8" target="_blank">
              Khavari, B., Ramirez, C., Jeuland, M. & Fuso Nerini, F. 
              “A geospatial approach to understanding clean cooking challenges in sub-Saharan Africa.” 
              <em>Nature Sustainability</em> (2023).
            </a>
          </li>
          <li>
            <a href="https://doi.org/10.1016/S2542-5196(24)00209-2" target="_blank">
              Ramirez, C. et al. 
              “Achieving Nepal’s clean cooking ambitions: an open source and geospatial cost–benefit analysis.” 
              <em>The Lancet Planetary Health</em> 8, e754–e765 (2024).
            </a>
          </li>
          <li>
            <a href="http://dx.doi.org/10.13140/RG.2.2.19033.29289" target="_blank">
              Khavari, B. et al. 
              “Integrated geospatial modelling for the achievement of universal energy access in Kenya.” 
              (2024).
            </a>
          </li>
        </ul>
      </div>

    </div>
  </div>
</section>

<section class="container-lg p-responsive py-4 py-md-6 my-lg-6">
  <div class="recommended-reading">
    <h2 class="alt-h2 text-center mb-4">Recommended Reading</h2>
    <p class="text-center mb-5">For a broader analysis of applications and advancements in OSeMOSYS, see the following peer-reviewed publications:</p>

    <div class="publications-list">
      {% for publication in site.data.publications %}
      <div class="publication-item mb-4 p-4 border border-gray-200 rounded">
        <h4 class="publication-title mb-2">
          <a href="{{ publication.url }}" target="_blank" class="text-decoration-none">
            {{ publication.title }}
          </a>
        </h4>
        <p class="publication-authors text-muted mb-2">
          {{ publication.authors }} ({{ publication.year }})
        </p>
        <p class="publication-journal mb-2">
          <em>{{ publication.journal }}</em>
        </p>
        <p class="publication-abstract text-justify">
          {{ publication.abstract }}
        </p>
      </div>
      {% endfor %}
    </div>

  </div>
  
</section>

<style>
/* Enhanced Applications Page Styling */
.applications-content {
  max-width: 1200px;
  margin: 0 auto;
}

.applications-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  margin-top: 2rem;
}

.application-category {
  background: white;
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
  transition: all 0.3s ease;
}

.application-category:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 25px rgba(0, 0, 0, 0.15);
}

.category-title {
  color: #0366d6;
  font-size: 1.3rem;
  font-weight: 600;
  margin-bottom: 1rem;
  padding-bottom: 0.5rem;
  border-bottom: 2px solid #e1e4e8;
}

.application-list {
  list-style: none;
  padding: 0;
  margin: 0;
}

.application-list li {
  margin-bottom: 0.8rem;
  padding-left: 1.5rem;
  position: relative;
}

.application-list li::before {
  content: "→";
  position: absolute;
  left: 0;
  color: #0366d6;
  font-weight: bold;
}

.application-list a {
  color: #24292e;
  text-decoration: none;
  transition: color 0.3s ease;
  line-height: 1.5;
}

.application-list a:hover {
  color: #0366d6;
  text-decoration: underline;
}

/* Enhanced Slider Styling */
.slider-wrapper {
  position: relative;
  max-width: 800px;
  margin: 0 auto;
  display: flex;
  align-items: center;
}

.slider-container {
  overflow: hidden;
  width: 100%;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

.slider {
  display: flex;
  transition: transform 0.6s ease-in-out;
}

.slide-card {
  min-width: 100%;
  padding: 2.5rem;
  background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
  border-left: 5px solid #0366d6;
  text-align: center;
  transition: all 0.3s ease;
}

.slide-card:hover {
  background: linear-gradient(135deg, #ffffff 0%, #f8f9fa 100%);
  transform: scale(1.02);
}

.slide-card h3 {
  margin-bottom: 1rem;
  color: #24292e;
  font-size: 1.5rem;
  font-weight: 600;
}

.slide-card a {
  color: #0366d6;
  text-decoration: none;
  font-weight: 500;
  font-size: 1.1rem;
  transition: all 0.3s ease;
}

.slide-card a:hover {
  color: #0056b3;
  text-decoration: underline;
}

.arrow {
  font-size: 2.5rem;
  cursor: pointer;
  user-select: none;
  padding: 0.5rem 1rem;
  color: #0366d6;
  background: rgba(255, 255, 255, 0.9);
  border-radius: 8px;
  transition: all 0.3s ease;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}

.arrow:hover {
  background: white;
  transform: scale(1.1);
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
}

.arrow-left {
  position: absolute;
  left: -50px;
}

.arrow-right {
  position: absolute;
  right: -50px;
}

.slider-dots {
  display: flex;
  justify-content: center;
  gap: 12px;
  margin-top: 1.5rem;
}

.slider-dots .dot {
  width: 12px;
  height: 12px;
  background-color: #d1d5da;
  border-radius: 50%;
  cursor: pointer;
  transition: all 0.3s ease;
}

.slider-dots .dot:hover {
  background-color: #0366d6;
  transform: scale(1.2);
}

.slider-dots .dot.active {
  background-color: #0366d6;
  transform: scale(1.2);
}

/* Enhanced Publications Styling */
.recommended-reading {
  max-width: 1000px;
  margin: 0 auto;
}

.publications-list {
  display: flex;
  flex-direction: column;
  gap: 2rem;
}

.publication-item {
  background: white;
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
  transition: all 0.3s ease;
  border-left: 4px solid #0366d6;
}

.publication-item:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 25px rgba(0, 0, 0, 0.15);
}

.publication-header {
  margin-bottom: 1rem;
}

.publication-title {
  font-size: 1.2rem;
  font-weight: 600;
  color: #24292e;
  margin-bottom: 0.5rem;
  line-height: 1.4;
}

.publication-authors {
  font-weight: 500;
  color: #586069;
  margin-bottom: 0.3rem;
}

.publication-journal {
  font-style: italic;
  color: #586069;
  margin-bottom: 0.5rem;
}

.publication-link {
  color: #0366d6;
  text-decoration: none;
  font-size: 0.9rem;
  word-break: break-all;
}

.publication-link:hover {
  text-decoration: underline;
}

.publication-abstract {
  color: #586069;
  line-height: 1.6;
  font-size: 0.95rem;
  text-align: justify;
}

/* Responsive Design */
@media (max-width: 768px) {
  .applications-grid {
    grid-template-columns: 1fr;
    gap: 1.5rem;
  }
  
  .application-category {
    padding: 1.5rem;
  }
  
  .arrow-left {
    left: -30px;
  }
  
  .arrow-right {
    right: -30px;
  }
  
  .slide-card {
    padding: 2rem 1.5rem;
  }
  
  .publication-item {
    padding: 1.5rem;
  }
}

@media (max-width: 480px) {
  .arrow {
    font-size: 2rem;
    padding: 0.3rem 0.8rem;
  }
  
  .arrow-left {
    left: -25px;
  }
  
  .arrow-right {
    right: -25px;
  }
}

/* Enhanced fade-in animations */
.fade-in-center {
  opacity: 0;
  transform: translateY(30px);
  animation: fadeInUp 1.2s ease-out forwards;
}

@keyframes fadeInUp {
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>

<script>
// Enhanced Slider Functionality
let slideIndex = 0;
const textSlider = document.getElementById("textSlider");
const textSlides = textSlider.children.length;
const dotsContainer = document.getElementById("sliderDots");

function updateSlider() {
  textSlider.style.transform = `translateX(-${slideIndex * 100}%)`;
  updateDots();
}

function slideTextNext() {
  slideIndex = (slideIndex + 1) % textSlides;
  updateSlider();
}

function slideTextPrev() {
  slideIndex = (slideIndex - 1 + textSlides) % textSlides;
  updateSlider();
}

function createDots() {
  for (let i = 0; i < textSlides; i++) {
    const dot = document.createElement("span");
    dot.classList.add("dot");
    dot.addEventListener("click", () => {
      slideIndex = i;
      updateSlider();
    });
    dotsContainer.appendChild(dot);
  }
}

function updateDots() {
  const dots = document.querySelectorAll(".slider-dots .dot");
  dots.forEach((dot, i) => {
    dot.classList.toggle("active", i === slideIndex);
  });
}

// Auto-slide functionality
let sliderInterval = setInterval(slideTextNext, 5000);

// Pause auto-slide on hover
textSlider.parentElement.addEventListener("mouseenter", () => {
  clearInterval(sliderInterval);
});

textSlider.parentElement.addEventListener("mouseleave", () => {
  sliderInterval = setInterval(slideTextNext, 5000);
});

// Keyboard navigation
document.addEventListener("keydown", (e) => {
  if (e.key === "ArrowLeft") {
    slideTextPrev();
  } else if (e.key === "ArrowRight") {
    slideTextNext();
  }
});

// Initialize
createDots();
updateSlider();
</script>
