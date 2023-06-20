<template>
  <div class="button-wrapper">
    <button
      v-if="asButton"
      class="button border-gradient"
      :class="{ 'button-secondary': isSecondary }"
      @click="generate"
    >
      {{ text }}
    </button>
    <a v-else :href="link" class="link border-gradient">{{ text }}</a>
  </div>
</template>
<script>
export default {
  name: "Button",
  props: {
    text: {
      type: String,
      default: "Generate",
    },
    asButton: {
      type: Boolean,
      default: true,
    },
    link: {
      type: String,
      default: "/",
    },
    isSecondary: {
      type: Boolean,
      default: false,
    },
  },
  methods: {
    generate() {
      this.$emit("generate");
    },
  },
};
</script>
<style scoped>
.button {
  background-color: var(--main-green-color);
  color: var(--background-color-main);
  font-size: var(--font-3xl);
  padding: 12px 1.125rem;
  border-radius: 4px;
  font-size: var(--font-md);
  font-weight: 600;
  cursor: pointer;
  border: none;
  border-radius: 5px;
}

.button-secondary {
  background-color: white;
  color: var(--background-color-main);
}
</style>



