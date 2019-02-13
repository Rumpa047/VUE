<template>
  <dir class="container">
    <div id="props" class="row">
      <div v-bind:key="item.id" v-for="item in data" class="col-xs-4 col-lg-4 box">
        <div class="thumbnail">
          <img class="img-resize" :src="item.img" alt="Image">

          <!-- <img
            class="lazy"
            src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT2F4bO2dX3Tf4FqbCdLu4dmGO4TgcpWQJuEoFKQ_N5H75Lv8Hv"
            :data-src="item.img"
            alt="Image"
          >-->
          <div class="text-box">
            <h3 class="title">{{item.name}}</h3>
          </div>
        </div>
      </div>
    </div>
  </dir>
</template>

<script>
export default {
  name: "ListView",
  props: ["data"]
};
</script>

<style scoped>
.back-img {
  background-color: rgb(217, 210, 224);
}
.img-resize {
  height: 300px;
  width: 300px;
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
</style>
