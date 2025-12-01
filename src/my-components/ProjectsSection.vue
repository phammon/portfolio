<template>
  <section class="py-5 bg-light" id="projects">
    <div class="container">
      <h2 class="title text-center mb-5">Projects</h2>
      <div class="row justify-content-center">
        <!-- Loop through projects -->
        <div
          v-for="(project, index) in projects"
          :key="index"
          class="col-md-6 col-lg-4 mb-4"
        >
          <div class="card shadow-sm h-100">
            <img
              :src="project.image"
              class="card-img-top"
              :alt="project.title"
            />
            <div class="card-body d-flex flex-column">
              <h5 class="card-title">{{ project.title }}</h5>
              <p class="card-text flex-grow-1">{{ project.description }}</p>
              <a
                :href="project.link"
                target="_blank"
                class="btn btn-outline-primary mt-3"
              >
                View Project
              </a>
            </div>
          </div>
        </div>
        <!-- End loop -->
      </div>
    </div>
  </section>
</template>

<script setup>
const projects = [
  {
    title: 'Reel Talk Coaching',
    description:
      'A fully responsive website built for a life coaching business, designed to showcase services, client testimonials, and provide an easy way for prospective clients to book sessions.',
    image: '/img/life-coach-website.png', // Replace with your actual screenshot
    link: 'https://www.reeltalkcoaching.com'
  },
  {
    title: 'Bodega Deals',
    description:
      'A CRM for managing and tracking real estate leads and deals. Built for speed, automation, and simplicity.',
    image: '/img/bodega-deals-dashboard.png',
    link: 'https://www.bodegadeals.com'
  },
  {
    title: 'Permit Pilot',
    description:
      'A comprehensive .NET Core/React application built for Fincher Services, a construction permitting and consulting company. Streamlines permit handling, licensing, project management, consulting, research, and notary services across 37+ Florida counties, with specialized focus on Marion County and surrounding areas.',
    image: '/img/permit-pilot-dashboard.png',
    link: 'https://www.permitpilot.app' // Update with actual project link if available
  },
  // Add more projects here
];
</script>
