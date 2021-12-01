<template>
  <div class="side-bar">
    <Drawer />
    <div class="side-bar__icons">
      <v-icon class="ico" icon="fa fa-book" size="large" />
      <p>projects</p>
    </div>
    <div class="side-bar__icons">
      <v-icon class="ico" icon="fa fa-archive" size="large" />
      <p>skill set</p>
    </div>
    <div class="side-bar__icons">
      <v-icon class="ico" icon="fa fa-user-alt" size="large" />
      <p>about</p>
    </div>
    <!--<div class="menu-ico">
      <v-icon  icon="fa fa-bars" />
    </div>-->
  </div>
</template>
<script>
import Drawer from "../layouts/SIdeDrawer.vue";

export default {
  name: "side bar",
  components: {
    Drawer,
  },
};
</script>
<style scoped>
.side-bar {
  width: 70px;
  float: left;
  position: absolute;
  background-color: white;
  padding: 10px;
  z-index: 2000;
  top: 20vh;
}
.side-bar__icons {
  color: gray;
  justify-content: center;
  margin-top: 20px;
}
.side-bar__icons > p {
  font-size: 10px;
  color: gray;
  text-align: center;
  padding-top: 10px;
}
.ico {
  padding-left: 7px;
  transition: transform 400ms;
}
.ico:hover {
  transform: scale(1.3, 1.3);
  color: rgb(220, 168, 255);
}
.menu-ico {
  bottom: 0;
}
</style>
