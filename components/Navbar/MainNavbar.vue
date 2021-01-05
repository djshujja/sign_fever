<template>
  <div class="middle-nav">
    <div class="row">
      <div class="col-1">
        <img class="logo" src="~/assets/logo-sf.svg" alt="" />
      </div>
      <div class="search col-5">
        <b-input-group class="mt-2">
          <b-form-input
            placeholder="What messages do you want on your sign?"
          ></b-form-input>
          <b-input-group-append>
            <b-button class="main-green">X</b-button>
          </b-input-group-append>
        </b-input-group>
      </div>
      <div class="col-2 row mt-2">
        <div class="col-4">
          <b-button class="main-green">X</b-button>
        </div>
        <div class="col-8">
          <h6>Chat Offline</h6>
          <small>Leave a Message</small>
        </div>
      </div>
      <div class="col-2 row mt-2">
        <div class="col-4">
          <b-button class="main-green">X</b-button>
        </div>
        <div class="col-8">
          <h6>Chat Offline</h6>
          <small>Leave a Message</small>
        </div>
      </div>
      <div class="col-2 row mt-2">
        <div class="col-4">
          <b-button class="main-green">X</b-button>
        </div>
        <div class="col-8">
          <h6>Chat Offline</h6>
          <small>Leave a Message</small>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
.middle-nav {
  background-color: #f3f3f3;
  padding: 10px 10px;
}
.main-green {
  background-color: var(--main-green);
}
</style>
