<template>
  <v-app class="main">
    <v-main>
      <Header />
      <Sidebar />
      <v-virtual-scroll height="100vh" item-height="100vh"> </v-virtual-scroll>
    </v-main>
  </v-app>
</template>

<script>
import Header from "./components/Header.vue";
import Sidebar from "./containers/SideBar.vue";

export default {
  name: "App",
  components: { Header, Sidebar },
  theme: { dark: true },
};
</script>
<style>
.main {
  background-color: rgb(228, 228, 228);
}
</style>
