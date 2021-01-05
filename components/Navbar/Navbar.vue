<template>
  <div>
    <UpperNav />
    <MainNav />
    <MenuNavbar />
  </div>
</template>
<script>
import UpperNav from "./UpperNav.vue";
import MainNav from "./MainNavbar";
import MenuNavbar from "./MenuNavbar";
export default {
  components: {
    UpperNav,
    MainNav,
    MenuNavbar
  }
};
</script>
<style scoped></style>
