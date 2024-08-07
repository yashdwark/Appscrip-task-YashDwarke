<template>
  <div>
    <NavBar />
    <ShopPage />
    <ItemsBar/>
    <FooterComponent/>
  </div>
</template>

<script>
import NavBar from '~/components/NavBar.vue';
import ShopPage from '~/components/ShopPage.vue';
import ItemsBar from '~/components/ItemsBar.vue';
import FooterComponent from '~/components/FooterComponent.vue';

export default {
  name: 'IndexPage',
  components: {
    NavBar,
    ShopPage,
    ItemsBar,
    FooterComponent
  }
}
</script>

<style scoped>
div{
  margin: 0;
  padding: 0;
}
</style>
