<template>
  <div id="app">
    <ListView v-bind:data="data_all"/>
  </div>
</template>

<script>
import ListView from "./components/ListView";

export default {
  name: "app",
  components: {
    ListView
  },
  data() {
    return {
      data_all: [
        {
          id: 1,
          name: "James",
          handle: "@jokerjames",
          img: "https://semantic-ui.com/images/avatar2/large/matthew.png",
          tweet: "If you don't succeed, dust yourself off and try again.",
          likes: 10
        },
        {
          id: 2,
          name: "Rat",
          handle: "@fantasticfatima",
          img: "https://semantic-ui.com/images/avatar2/large/molly.png",
          tweet: "Better late than never but never late is better.",
          likes: 12
        },
        {
          id: 3,
          name: "Xin",
          handle: "@xeroxin",
          img: "https://semantic-ui.com/images/avatar2/large/elyse.png",
          tweet: "Beauty in the struggle, ugliness in the success.",
          likes: 18
        }
      ]
    };
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
