<template>
  <div class="drawer">
    <div class="drawer__top">
      <img :src="require('../assets/avatar.jpg')" alt="" />
    </div>
  </div>
</template>
<script>
import { createVuetify } from "vuetify";

export default createVuetify({
  name: "drawer",
});
</script>
<style>
.drawer__top > img {
  height: 40px;
}
</style>
