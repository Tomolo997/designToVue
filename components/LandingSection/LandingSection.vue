<template>
  <section class="landing-section">
    <div class="landing-section-wrapper">
      <h1 class="landing-section-h1">Unlimited</h1>
      <h1 class="landing-section-h1">
        <span class="design-span">Design</span> to
        <span class="vue-code-span">Vue Code</span>
      </h1>
      <p>
        — Unlock your business’s full potential with expert Vue development.
      </p>
      <ul class="landing-section-list">
        <li><Icon name="material-symbols:check-box" />Flat monthly fee</li>
        <li><Icon name="material-symbols:check-box" />Cancel at any time</li>
        <li><Icon name="material-symbols:check-box" />No contracts</li>
        <li>
          <Icon name="material-symbols:check-box" /> Ongoing or one-time
          development needs
        </li>
      </ul>
    </div>
  </section>
</template>
  <script>
export default {};
</script>
  <style scoped>
.landing-section {
  width: var(--container-width);
  height: 60vh;
  display: flex;
  align-items: center;
  justify-content: center;
}
.landing-section-list {
  list-style: none;
  padding: 0;
  margin: 0;
}
.landing-section-h1 {
  font-size: 5rem;
}
.landing-section-wrapper {
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
}
.design-span {
  color: transparent;
  background-image: linear-gradient(to top, #0047e1, #36e4da, #0047e1);
  -webkit-background-clip: text;
  background-clip: text;
}
.vue-code-span {
  color: transparent;
  background-image: linear-gradient(to top, #00dc82, #36e4da, #00dc82);
  -webkit-background-clip: text;
  background-clip: text;
}
</style>