<template>
  <dir>
    <h1>hello</h1>
    <dir v-bind:key="item.id" v-for="item in data">
      <h3>{{item.title}}</h3>
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
</style>
