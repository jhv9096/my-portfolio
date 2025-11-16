<script setup>
defineOptions({ name: 'IntroBlock' })
</script>

<template>
  <section class="intro-block" role="region" aria-labelledby="intro-heading">
    <div class="intro-content">
      <h1 id="intro-heading" class="intro-title">
        Hi, I'm John Vander Linden — Software Engineer
      </h1>

      <p class="intro-sub">
        I'm a recent graduate from RIT looking to make positive change in the world through programming, ensuring that the digital tools people use serve their intended purpose with as little downtime as possible.
      </p>

      <div class="intro-actions">
        <router-link class="btn btn-primary" to="/projects">View Projects</router-link>
        <router-link class="btn btn-outline" to="/contact">Get in Touch</router-link>
      </div>

      <ul class="intro-meta" aria-hidden="true">
        <li>Java</li>
        <li>Spring • SpringBoot</li>
        <li>Python</li>
        <li>C#</li>
        <li>PostgreSQL</li>
        <li>Vue 3 • Vite</li>
        <li>HTML • CSS • JavaScript</li>
<!--        <li>Responsive & Accessible UI</li>-->
      </ul>
    </div>
  </section>

</template>

<style scoped>
.intro-block {
  padding: 3rem 1rem;
  background: var(--color-bg, #f9f9f9);
  display: flex;
  justify-content: center;
}

.intro-content {
  max-width: 960px;
  width: 100%;
  text-align: center;
}

.intro-title {
  font-size: clamp(2rem, 5vw, 3rem);
  margin-bottom: 1rem;
  color: var(--color-text, #0f1720);
}

.intro-sub {
  font-size: 1.1rem;
  color: var(--color-muted, #6b7280);
  margin-bottom: 2rem;
  max-width: 60ch;
  margin-inline: auto;
}

.intro-actions {
  display: flex;
  gap: 1rem;
  justify-content: center;
  margin-bottom: 1.5rem;
}

.btn {
  padding: 0.75rem 1.25rem;
  border-radius: 6px;
  font-weight: 600;
  text-decoration: none;
  font-size: 0.95rem;
  border: 1px solid transparent;
}

.btn-primary {
  background: var(--color-accent, #0ea5a4);
  color: white;
}

.btn-outline {
  background: transparent;
  color: var(--color-text, #0f1720);
  border: 1px solid rgba(15, 23, 32, 0.1);
}

.intro-meta {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
  gap: 1rem;
  justify-content: center;
  font-size: 0.9rem;
  color: var(--color-muted, #6b7280);
  flex-wrap: wrap;
}
</style>

