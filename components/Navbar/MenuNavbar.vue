<template>
  <div>
    <b-nav class="menu-navbar">
      <b-nav-item>Home</b-nav-item>
      <b-nav-item>Social Distancing</b-nav-item>
      <b-nav-item>Custom</b-nav-item>
      <b-nav-item>OSHA / ANSI</b-nav-item>
      <b-nav-item>Personal Protection</b-nav-item>
      <b-nav-item>Electrical</b-nav-item>
      <b-nav-item>Chemical</b-nav-item>
      <b-nav-item>Construction</b-nav-item>
      <b-nav-item>Fire</b-nav-item>
    </b-nav>
    <div class="learn-more text-center">
      <i><u>Social Distancing Signs</u> – Learn More</i>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
.menu-navbar {
  background-color: var(--main-green);
  & > * > * {
    color: white;
    margin-right: 30px;
  }
  & > * {
    border-right: 1px solid rgb(56, 56, 56);
  }
  & > *:hover {
    background-color: #355588;
    border-right: 1px solid rgb(56, 56, 56);
  }
}
.learn-more {
  background-color: #ffffcc;
  color: #cc0000;
  font-size: 1.2rem;
  font-weight: 500;
  padding: 5px 0px;
  border-bottom: 2px solid var(--main-green);
}
</style>
