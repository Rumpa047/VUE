<template>
  <dir class="back-img">
    <!-- <h1>hello</h1> -->
    <dir v-bind:key="item.id" v-for="item in data">
      <h3>{{item.name}}</h3>
      <figure>
        <img :src="item.img" alt="Image">
      </figure>
    </dir>
  </dir>
</template>

<script>
export default {
  name: "ListView",
  props: ["data"]
};
</script>

<style scoped>
html,
body {
  height: 100%;
  padding-top: 10px;
  background-image: blue;
}
.back-img {
  background-color: rgb(217, 210, 224);
}

img {
  border-radius: 30px;
  height: 200px;
  width: 200px;
}
/* .content small {
  color: #00d1b2;
}

.likes {
  padding: 0 7.5px;
} */
</style>
