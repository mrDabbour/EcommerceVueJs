<template>
  <div class="layout">
    <v-layout>
      <v-navigation-drawer v-model="drawer" location="right">
        <b>Cart</b>
      </v-navigation-drawer>
      <v-main>
        <h1>Ecommerce Project</h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. FDoloribus ex
          earum pariatur consectetur lab ore officiis distinct io, perferendis
          laboriosa m quo. Cupiditate sed sapiente corrupti impedit in quam
          minus beatae facilis facere?
        </p>
      </v-main>
      <v-app-bar>
        <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>
      </v-app-bar>
      <v-footer :app="true">
        <p>Mohammed Dabour Website</p>
      </v-footer>
    </v-layout>
  </div>
</template>
<script>
export default {
  data() {
    return {
      drawer: true,
    };
  },
};
</script>
