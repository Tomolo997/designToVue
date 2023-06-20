<template>
  <section class="landing-section">
    <div class="landing-section-wrapper">
      <h1 class="landing-section-h1">Unlimited</h1>
      <div class="landing-section-design-to-vue-div">
        <span class="landing-section-h1 design-span">Design</span>
        <span class="to-span"> to </span>
        <span class="landing-section-h1 vue-code-span">Vue Code</span>
      </div>
      <p class="description">
        — Unlock your business’s full potential with expert Vue development.
      </p>
      <ul class="landing-section-list">
        <li class="landing-section-list-item">
          <Icon
            class="landing-section-list-item-logo"
            name="material-symbols:check-box"
          />Flat monthly fee
        </li>
        <li class="landing-section-list-item">
          <Icon
            class="landing-section-list-item-logo"
            name="material-symbols:check-box"
          />Cancel at any time
        </li>
        <li class="landing-section-list-item">
          <Icon
            class="landing-section-list-item-logo"
            name="material-symbols:check-box"
          />No contracts
        </li>
        <li class="landing-section-list-item">
          <Icon
            class="landing-section-list-item-logo"
            name="material-symbols:check-box"
          />
          Ongoing or one-time development needs
        </li>
      </ul>
      <div class="buttons">
        <ButtonMain :text="'See how pricing works'" />
        <ButtonMain :isSecondary="true" :text="'What is our process'" />
      </div>
    </div>
  </section>
</template>
  <script>
import ButtonMain from "../Utils/ButtonMain.vue";
export default {
  name: "LandingSection",
  components: {
    ButtonMain,
  },
  methods: {},
};
</script>
  <style scoped>
.landing-section {
  width: var(--container-width);
  height: 80vh;
  display: flex;
  align-items: center;
  justify-content: center;
}
.landing-section-list {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
  gap: 2.5rem;
  margin-top: 3rem;
}
.landing-section-list-item {
  font-size: var(--font-md);
  display: flex;
  align-items: center;
  color: var(--text-on-background-color-whiter);
}
.landing-section-list-item-logo {
  margin-right: 4px;
  font-size: var(--font-2xl);
}
.landing-section-h1 {
  font-size: var(--font-6xl);
  font-weight: 600;
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
  font-weight: 600;
}
.vue-code-span {
  color: transparent;
  background-image: linear-gradient(to top, #00dc82, #36e4da, #00dc82);
  -webkit-background-clip: text;
  background-clip: text;
  font-weight: 600;
}
.to-span {
  font-size: var(--font-4xl);
  text-align: start;
  font-weight: 600;
  margin-left: 12px;
  margin-right: 12px;
}
.landing-section-design-to-vue-div {
  display: flex;
  justify-content: center;
  align-items: center;
}

.description {
  color: var(--text-on-background-color);
  font-size: var(--font-lg);
  margin-top: 2rem;
}
.buttons {
  margin-top: 3.5rem;
  display: flex;
  gap: 1rem;
}
</style>