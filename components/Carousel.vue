<template>
  <div>
    <!-- v-model="dots" -->
    <b-carousel
      id="carousel-1"
      :interval="4000"
      controls
      indicators
      background="#ababab"
      img-width="1024"
      img-height="480"
      style="text-shadow: 1px 1px 2px #333;"
    >
      <!-- @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd" -->
      <!-- Text slides with image -->
      <b-carousel-slide
        img-src="https://images.mysafetysign.com/img/dp/md/custom-signs-templates.jpg"
      ></b-carousel-slide>

      <!-- Slides with custom text -->
      <b-carousel-slide
        img-src="https://images.mysafetysign.com/img/dp/md/custom-safety-signs.jpg"
      >
      </b-carousel-slide>

      <!-- Slides with image only -->
      <b-carousel-slide
        img-src="https://picsum.photos/1024/480/?image=58"
      ></b-carousel-slide>

      <!-- Slides with img slot -->
      <!-- Note the classes .d-block and .img-fluid to prevent browser default image alignment -->
    </b-carousel>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped></style>
