<template>
  <b-row>
    <b-col>
      <div>
        <img :src="selectedDesign.thumbnail" alt="" width="350" height="350" />
        <h5>{{ selectedDesign.title }}</h5>
      </div>
    </b-col>
    <b-col class="variations-col" cols="8">
      <div>
        <h4>
          {{ product.name }}
        </h4>
      </div>
      <div>
        <h5>1. Select Design</h5>
        <b-row cols="5">
          <b-col
            v-for="design in product.designs"
            :key="design.title"
            @click="selectDesign(design)"
          >
            <img
              class="cursor-pointer"
              :src="design.thumbnail"
              alt=""
              width="75%"
              height="75%"
            />
            <h6 class="cursor-pointer">{{ design.title }}</h6>
          </b-col>
        </b-row>
      </div>
      <div>
        <h5>2. Select Size</h5>
        <b-row cols="5" class="justify-center">
          <b-col v-for="size in selectedDesign.sizes" :key="size.title">
            <div @click="selectSize(size)" class="w-100 border cursor-pointer">
              {{ size.size }}
            </div>
          </b-col>
        </b-row>
      </div>
      <div>
        <h5>3. Select Material</h5>
        <b-row v-for="material in selectedSize.materials" :key="material.name">
          <b-col>{{ material.name }} - {{ material.price }}</b-col>
        </b-row>
      </div>
    </b-col>
  </b-row>
</template>

<script>
export default {
  props: ["product"],

  data() {
    return {
      selectedDesign: {},
      selectedSize: {},
      selectedMaterial: {},
      productData: {}
    };
  },

  mounted() {
    this.selectedDesign = this.product.designs[0];
    console.log(this.selectedDesign);
    this.selectedSize = this.selectedDesign.sizes[0];
    console.log(this.selectedSize);
  },
  methods: {
    selectDesign(design) {
      this.selectedDesign = design;
      this.selectedSize = design.sizes;
    },
    selectSize(size) {
      this.selectedSize = size;
    },
    selectMaterial(material) {
      this.selectedMaterial = material;
    }
  }
};
</script>

<style lang="scss" scoped>
.variations-col {
}
.cursor-pointer:hover {
  cursor: pointer;
}
</style>
