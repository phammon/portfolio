<template>
  <section class="py-5 bg-light" id="contact">
    <div class="container">
      <div class="row justify-content-center text-center">
        <div class="col-lg-8">
          <h2 class="title">Contact Me</h2>
          <p class="description">Have a project in mind or just want to connect? Drop me a message below!</p>
          <form @submit.prevent="submitForm">
            <div class="mb-3">
              <input type="text" v-model="form.name" class="form-control" placeholder="Your Name" required />
            </div>
            <div class="mb-3">
              <input type="email" v-model="form.email" class="form-control" placeholder="Your Email" required />
            </div>
            <div class="mb-3">
              <textarea v-model="form.message" class="form-control" placeholder="Your Message" rows="5" required></textarea>
            </div>
            <button type="submit" class="btn btn-primary">Send Message</button>
          </form>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue';

const form = ref({ name: '', email: '', message: '' });

const submitForm = () => {
  const subject = encodeURIComponent(`Message from ${form.value.name}`);
  const body = encodeURIComponent(
    `Name: ${form.value.name}\nEmail: ${form.value.email}\n\n${form.value.message}`
  );
  const mailtoLink = `mailto:phammonn@gmail.com?subject=${subject}&body=${body}`;

  window.location.href = mailtoLink;

  // Reset the form after sending
  form.value = { name: '', email: '', message: '' };
};
</script>
