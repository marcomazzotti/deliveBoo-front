<script>
import NavHeader from './components/NavHeader.vue';
import AppFooter from './components/AppFooter.vue';
import Cart from './components/Cart.vue';
import { store } from './store';
export default {
  data () {
    return {
      store,
    }
  },
  components: { NavHeader, AppFooter, Cart }
};
</script>

<template>
  <NavHeader />
  <Cart />

  <router-view />

  <AppFooter />
</template>

<style lang="scss">
@use "./styles/general.scss";
</style>