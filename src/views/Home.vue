<template>
  <div>
    <Navbar />
    <HeroSection />
    <ServicesSection />
    <AboutSection />
    <ProjectsSection />
    <ContactSection />
    <!-- <DefaultFooter /> -->
  </div>
</template>

<script setup>
import Navbar from "@/my-components/Navbar.vue"
import HeroSection from "@/my-components/HeroSection.vue"
import AboutSection from "@/my-components/AboutSection.vue"
import ProjectsSection from "@/my-components/ProjectsSection.vue"
import ContactSection from "@/my-components/ContactSection.vue"
import ServicesSection from "@/my-components/ServicesSection.vue"
</script>
