<template>
     <section class="py-5 bg-light" id="services">
    <div class="container">
      <h2 class="title text-center mb-5">What I Can Help You With</h2>
      <div class="row g-4 justify-content-center">
        <!-- Card 1 -->
        <div class="col-md-4">
          <div
            class="card shadow-sm service-card d-flex flex-column align-items-center text-center px-4 py-5"
          >
            <span class="material-icons md-48 text-primary mb-3">code</span>
            <h5 class="card-title mb-3">Software & Web Development</h5>
            <ul class="list-unstyled mb-0 text-muted">
              <li>• Custom websites, CRMs, and dashboards</li>
              <li>• Mobile-friendly and responsive design</li>
              <li>• Mobile app development (iOS & Android)</li>
              <li>• Built with Vue.js, .NET, Node.js & more</li>
            </ul>
          </div>
        </div>

        <!-- Card 2 -->
        <div class="col-md-4">
          <div
            class="card shadow-sm service-card d-flex flex-column align-items-center text-center px-4 py-5"
          >
            <span class="material-icons md-48 text-primary mb-3">wifi</span>
            <h5 class="card-title mb-3">IT Support & Networking</h5>
            <ul class="list-unstyled mb-0 text-muted">
              <li>• Setup for workstations and Wi-Fi networks</li>
              <li>• Troubleshoot printers, systems, and more</li>
              <li>• Focused on security, reliability, and speed</li>
            </ul>
          </div>
        </div>

        <!-- Card 3 -->
        <div class="col-md-4">
          <div
            class="card shadow-sm service-card d-flex flex-column align-items-center text-center px-4 py-5"
          >
            <span class="material-icons md-48 text-primary mb-3">business</span>
            <h5 class="card-title mb-3">Business Tech Consulting</h5>
            <ul class="list-unstyled mb-0 text-muted">
              <li>• Find smarter ways to run your business</li>
              <li>• Automate tasks, improve workflows</li>
              <li>• Translate business needs into tech solutions</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
.service-card {
  min-height: 320px; /* taller, less squat */
  border-radius: 15px;
  transition: box-shadow 0.3s ease;
}

.service-card:hover {
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.12);
}

.material-icons.md-48 {
  font-size: 48px;
}

/* Optional: adjust bullet spacing and color */
/* ul.list-unstyled li {
  margin-bottom: 0.5rem;
  color: #6c757d;
} */
</style>