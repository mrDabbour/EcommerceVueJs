<template>
  <div class="layout">
    <v-layout>
      <cart-drawer></cart-drawer>
      <app-nav></app-nav>
      <v-main>
        <h1>Ecommerce Project</h1>
        <slot></slot>
      </v-main>
      <app-footer></app-footer>
    </v-layout>
  </div>
</template>
<script>
import AppNav from "./AppNav";
import AppFooter from "./AppFooter";
import CartDrawer from "./CartDrawer.vue";
// @click="drawer = true"

export default {
  data() {
    return {
      drawer: true,
    };
  },
  components: {
    AppFooter,
    AppNav,
    CartDrawer,
  },
};
</script>
