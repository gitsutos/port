<template>
  <div class="header">
    <div class="header__left">
      <div class="header__logo">
        <img v-bind:src="require('../assets/logo.png')" alt="" />
      </div>
      <div class="header__search">
        <v-icon icon="fa-search fa fa-search" />
        <input type="text" placeholder="Search" />
      </div>
    </div>
    <div class="header__right"></div>
  </div>
</template>
<script>
import "@fortawesome/fontawesome-free/css/all.css";
import { createVuetify } from "vuetify";
import Logo from "../assets/logo.png";
import { aliases, fa } from "vuetify/iconsets/fa";

export default createVuetify({
  name: "Header",
  /*  components: {
      HelloWorld,
    },*/
  data() {
    return {
      Logo: Logo,
    };
  },
  icons: {
    defaultSet: "fa",
    aliases,
    sets: {
      fa,
    },
  },
});
</script>
<style lang="css" scoped>
.header {
  display: flex;
  background: linear-gradient(to top, rgb(0, 75, 144), rgb(0, 115, 196));
  animation: mymove 5s infinite;
  transition: transform 1000ms;
  padding: 14px;
}
.header__left {
  display: flex;
}
.header__search {
  padding: 10px;
  background-color: rgb(226, 226, 226);
  border-radius: 40px;
}
.fa-search {
  color: gray;
  margin-right: 10px;
}
.header__search > input {
  border: none 0, 0, 0, 0;
  background-color: transparent;
  border-width: 0px;
  height: 25px;
  color: gray;
}
.header__logo > img {
  height: 30px;
}
.header__logo {
  margin-right: 4vw;
  margin-left: 4vw;
  background: linear-gradient(
    to bottom,
    rgba(255, 255, 255, 0.486),
    rgba(216, 216, 216, 0.555)
  );
  border-top-right-radius: 20px;
  border-bottom-left-radius: 20px;
  padding-right: 10px;
  padding-left: 10px;
  padding-top: 6px;
  transition: transform 300ms;
}
.header__logo:hover {
  transform: scale(1.2, 1.2);
  background-color: rgb(221, 221, 221);
}
</style>
