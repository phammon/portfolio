<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-white shadow-sm py-2 px-3">
    <div class="container">
      <a href="#" class="navbar-brand font-weight-bold text-dark">
        My Portfolio
      </a>

      <button
        class="navbar-toggler"
        type="button"
        @click="toggleNavbar"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" :class="{ show: navbarOpen }" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item" v-for="(link, index) in navLinks" :key="index">
            <a
              class="nav-link"
              :href="link.href"
              @click="navbarOpen = false"
            >
              {{ link.label }}
            </a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script setup>
import { ref } from 'vue';

const navbarOpen = ref(false);

const navLinks = [
  { label: 'Home', href: '#' },
  { label: 'About', href: '#about' },
  { label: 'Projects', href: '#projects' },
  { label: 'Contact', href: '#contact' }
];
</script>

<style scoped>
.navbar-nav .nav-link {
  padding-left: 1rem;
  padding-right: 1rem;
  font-weight: 500;
  color: #344767;
  transition: color 0.3s ease;
  cursor: pointer;
}
.navbar-nav .nav-link:hover {
  color: #007bff;
}
</style>
