<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';



export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter,
  },

  data() {
    return {
      links: ["Characters", "Comics", "Movies", "TV", "Games", "Collectibles", "Videos", "Fans", "News", "Shop"],
      images: [{
          name: "Digital Comics",
          path: "./src/assets/img/buy-comics-digital-comics.png",
        },
        {
          name: "Dc Merchandise",
          path: "./src/assets/img/buy-comics-merchandise.png",
        },
        {
          name: "Subscription",
          path: "./src/assets/img/buy-comics-subscriptions.png",
        },
        {
          name: "Comic Shop Locator",
          path: "./src/assets/img/buy-comics-shop-locator.png",
        },
        {
          name: "Dc Power Visa",
          path: "./src/assets/img/buy-dc-power-visa.svg",
        },
      ],
    }
  },
  methods: {
    
  }
}
</script>


<template>
<div>
  <AppHeader :links="links" />

  <AppMain :images="images" />

  <AppFooter :links="links" />

</div>

</template>

<style scoped>

</style>
