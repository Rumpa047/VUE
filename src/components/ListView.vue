<template>
  <div id="props">
    <div
      v-bind:key="item.id"
      v-for="item in data"
      :class="groupWrapper"
      class="col-xs-4 col-lg-4 box"
    >
      <div class="thumbnail">
        <img :src="item.img" alt="Image">
        <h3 class="title">{{item.name}}</h3>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ListView",
  groupWrapper: "list-group-item",
  props: ["data"]
};
</script>

<style scoped>
.back-img {
  background-color: rgb(217, 210, 224);
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
.title {
  text-align: left;
  padding-left: 5%;
  font-family: "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS", sans-serif;
  font-style: italic;
}
</style>
