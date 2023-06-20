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
    <div class="header-border-bottom"></div>
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
  background-image: linear-gradient(
    90deg,
    rgba(116, 123, 155, 0),
    var(--main-green-color) 50%,
    rgba(116, 123, 155, 0)
  );
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
  font-size: var(--font-2xl);
  font-weight: 600;
  color: #fff;
  text-align: center;
  line-height: 80px;
}
.logo {
  color: var(--main-green-color);
  font-style: none;
  font-size: var(--font-md);
}
.logo-to {
  color: white;
}
.logo-name {
  font-style: italic;
}
.header-border-bottom {
  position: absolute;
  top: 80px;
  z-index: 1;
  width: 100%;
  height: 1px;
  background: linear-gradient(
    90deg,
    rgba(116, 123, 155, 0),
    var(--main-green-color) 50%,
    rgba(116, 123, 155, 0)
  );
}
</style>