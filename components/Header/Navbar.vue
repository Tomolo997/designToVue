<template>
  <header>
    <div class="gradient"></div>
    <div class="header-wrapper">
      <div></div>
      <div class="header-logo">
        <span class="logo">D<span class="logo-to">to</span>V</span>
        <span class="logo-name"> DesignToVue </span>
      </div>
      <div class="header-login">Log in</div>
    </div>
  </header>
</template>
<script>
export default {};
</script>
<style scoped>
header {
  position: fixed;
  width: 100%;
  height: 80px;
  background-color: #10231531;
  backdrop-filter: blur(4px);
  display: flex;
  justify-content: center;
  align-items: center;
}
.gradient {
  background-image: linear-gradient(45deg, #00dc82, #36e4da, #0047e1);
  filter: blur(60px);
  z-index: -1;
  position: absolute;
  width: 100%;
  height: 30px;
  filter: blur(60px);
}
.header-wrapper {
  width: var(--container-width);
  height: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.header-logo {
  font-size: 1.5rem;
  font-weight: 600;
  color: #fff;
  text-align: center;
  line-height: 80px;
}
.logo {
  color: var(--main-green-color);
  font-style: none;
  font-size: 1rem;
}
.logo-to {
  color: white;
}
.logo-name {
  font-style: italic;
}
</style>