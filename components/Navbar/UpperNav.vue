<template>
  <div class="upper-nav">
    <ul>
      <li><a href="#">My Account</a></li>
      <li><a href="#">Customer Service</a></li>
      <li>
        <a href="#"
          ><b>Free Shipping</b> for order of $29.95 and more.
          <b>Free 2nd Day UPS</b> for order of $100 or more</a
        >
      </li>
    </ul>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
.upper-nav {
  font-size: 0.8rem;
  padding-top: 5px;
  border-bottom: 1px solid #636363;
  color: #636363;
  ul {
    list-style: none;
    display: flex;
    * > * {
      margin: 2px 6px;
    }
  }
  a {
    text-decoration: none;
    color: black;
  }
}
</style>
