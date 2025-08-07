<template>
  <section class="py-5 bg-light" id="projects">
    <div class="container">
      <h2 class="title text-center mb-5">Projects</h2>
      <div class="row justify-content-center">
        <div class="col-md-6">
          <div class="card shadow-sm">
            <img :src="project.image" class="card-img-top" :alt="project.title" />
            <div class="card-body">
              <h5 class="card-title">{{ project.title }}</h5>
              <p class="card-text">{{ project.description }}</p>
              <a :href="project.link" target="_blank" class="btn btn-outline-primary">
                View Project
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const project = {
  title: 'Bodega Deals',
  description: 'A CRM for managing and tracking real estate leads and deals. Built for speed, automation, and simplicity.',
  image: '/img/bodega-deals-dashboard.png', // Replace with actual screenshot if you have one
  link: 'https://www.bodegadeals.com'
};
</script>
