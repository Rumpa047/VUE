<template>
  <dir class="container">
    <div id="props" class="row">
      <div v-bind:key="item.id" v-for="item in data" class="col-xs-4 col-lg-4 box">
        <div class="thumbnail">
          <v-lazy-image class="img-resize" :src="item.img"/>

          <div class="text-box">
            <h3 class="title">{{item.name}}</h3>
          </div>
        </div>
      </div>
    </div>
  </dir>
</template>

<script>
import VLazyImage from "v-lazy-image";

export default {
  name: "ListView",
  props: ["data"],
  components: {
    VLazyImage
  }
};
</script>

<style scoped>
.back-img {
  background-color: rgb(217, 210, 224);
}
.img-resize {
  height: 300px;
  /* width: 300px; */
}
img {
  padding-top: 10px;
  border-radius: 5px;
  height: 80%;
  width: 95%;
}
.box {
  padding: 20px;
}
.text-box {
  padding-top: 5px;
  height: 100px;
  width: 100%;
}
.title {
  text-align: left;
  padding-left: 5%;
  font-family: "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS", sans-serif;
  font-style: italic;
  font-size: 1.2vw;
}
.v-lazy-image {
  filter: blur(10px);
  transition: filter 10s;
}
.v-lazy-image-loaded {
  filter: blur(0);
}
</style>
