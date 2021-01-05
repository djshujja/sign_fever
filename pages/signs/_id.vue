<template>
  <div class="mt-5 mx-5">
    <ProductDetails :product="Product" />
  </div>
</template>

<script>
import ProductDetails from "~/components/Product/Details/ProductDetails";
export default {
  components: {
    ProductDetails
  },
  computed: {
    Product() {
      return {
        name: "Custom OSHA Danger Sign: Add Your Own Wording Here",
        category: "main",
        "sub-categories": "subs",
        designs: [
          {
            title: "S-3057",
            thumbnail:
              "https://images.mysafetysign.com/img/lg/S/Custom-Danger-Sign-S-3136.gif",
            pictures: ["img-src-1-1", "img-src-1-2", "img-src-1-3"],
            sizes: [
              {
                title: "size-1",
                size: "2.25 x 648",
                materials: [
                  {
                    name: "plastic",
                    price: 50.5
                  },
                  {
                    name: "alimunium",
                    price: 80.5
                  },
                  {
                    name: "wood",
                    price: 150.5
                  }
                ]
              },
              {
                title: "size-2",
                size: "3.25 x 848",
                materials: [
                  {
                    name: "plastic",
                    price: 50.5
                  },
                  {
                    name: "alimunium",
                    price: 80.5
                  }
                ]
              }
            ]
          },
          {
            title: "S-4086",
            thumbnail:
              "https://images.mysafetysign.com/img/lg/S/Custom-Danger-Sign-S-3082.gif",
            pictures: ["img-src-1-1", "img-src-1-2", "img-src-1-3"],
            sizes: [
              {
                title: "size-1",
                size: "10.25 x 648",
                materials: [
                  {
                    name: "plastic",
                    price: 50.5
                  },
                  {
                    name: "alimunium",
                    price: 80.5
                  }
                ]
              },
              {
                title: "size-2",
                size: "50.25 x 848",
                materials: [
                  {
                    name: "laminated plastic",
                    price: 150.5
                  }
                ]
              }
            ]
          }
          // {
          //   title: "def",
          //   thumbnail:
          //     "https://images.mysafetysign.com/img/lg/S/Custom-Danger-Sign-S-3082.gif",
          //   pictures: ["img-src-2-1", "img-src-2-2", "img-src-2-3"],
          //   sizes: [
          //     {
          //       title: "size-1",
          //       size: "2.25 x 648",
          //       materials: [
          //         {
          //           name: "plastic",
          //           price: 20.5
          //         },
          //         {
          //           name: "alimunium",
          //           price: 40.5
          //         }
          //       ]
          //     },
          //     {
          //       title: "size-2",
          //       size: "3.25 x 848",
          //       materials: [
          //         {
          //           name: "plastic",
          //           price: 50.5
          //         },
          //         {
          //           name: "alimunium",
          //           price: 80.5
          //         }
          //       ]
          //     }
          //   ]
          // }
        ]
      };
    }
  }
};
</script>

<style lang="scss" scoped></style>
