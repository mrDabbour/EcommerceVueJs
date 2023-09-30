<template>
  <div class="drawer">
    <v-navigation-drawer v-model="drawer" location="right">
      <b>Cart</b>
    </v-navigation-drawer>
  </div>
</template>
<script>
export default {
  inject: ["Emitter"],
  data: () => ({
    drawer: false,
  }),
  mounted() {
    this.Emitter.on("openCart", () => {
      this.drawer = true;
    });
  },
};
</script>
