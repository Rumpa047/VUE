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
          name: "Beautiful Golf Course View Villa.Rainbow Inn Aiea.",
          img:
            "https://odis.homeaway.com/odis/listing/f548e387-7057-44f6-82ca-cbb567c0472b.c10.jpg"

          // "https://odis.homeaway.com/odis/listing/821e8093-8094-425b-9386-c36b940f9611.c10.jpg"
          // "https://odis.homeaway.com/odis/listing/661db966-569e-4cb4-8ea7-46eff97af432.c10.jpg"
        },
        {
          id: 2,
          name:
            "Private, Romantic Cottage On An Estate Property In The Hamakua District",
          img:
            "https://odis.homeaway.com/odis/listing/93623172-1288-475b-bc63-57c36c919d86.c10.jpg"
          // "https://odis.homeaway.com/odis/listing/f548e387-7057-44f6-82ca-cbb567c0472b.c10.jpg"
        },
        {
          id: 3,
          name:
            "Spacious Ilikai Studio with one FREE parking/WiFi and Marina/Ocean Views!",
          img:
            "https://odis.homeaway.com/odis/listing/d6855dd9-21a7-4553-8976-02196a051ab3.c10.jpg"
        },
        {
          id: 4,
          name:
            "Rainbow Inn Aiea. Overlooking Pearl Harbor. Discounts may be available.",
          img:
            "https://odis.homeaway.com/odis/listing/5d60c144-8cb8-47e5-be52-ed6abb4c4a24.c10.jpg"
        },
        {
          id: 5,
          name: "Incredible New Luxury Home inside the Mauna Lani Resort",
          img:
            "https://odis.homeaway.com/odis/listing/7f033ddb-b2a2-4155-b3f1-226f3b70f064.c10.jpg"
        },
        {
          id: 6,
          name:
            'Hawaii Life Presents "Kulani" of the Mahana- The Reserve Collection',
          img:
            "https://odis.homeaway.com/odis/listing/34a5aade-9bff-45cf-ab59-1b2b71b3858e.c10.jpg"
        },
        {
          id: 7,
          name: "Book the Whole House In Hawaii...",
          img:
            "https://odis.homeaway.com/odis/listing/8cbb6a7f-28b1-47b2-a9d2-6779d0a8cb46.c10.jpg"
        },
        {
          id: 8,
          name: "Air conditioned townhouse In hear",
          img:
            "https://odis.homeaway.com/odis/listing/d62a8873-91f9-4060-827a-2fbb2a035a14.c9.jpg"
        },
        {
          id: 9,
          name: "Cozy Volcano Studio",
          img:
            "https://odis.homeaway.com/odis/listing/53d80660-8e02-4987-ba34-98da22969f04.c9.jpg"
        },
        {
          id: 10,
          name: "Simple Kona Guest House",
          img:
            "https://odis.homeaway.com/odis/listing/37ab686a-79ef-4ccd-b69b-606b68f5b16d.c10.jpg"
        },
        {
          id: 11,
          name: "Kepuhi Beach End Condo ",
          img:
            "https://a0.muscache.com/im/pictures/88137054/c9f021a2_original.jpg?aki_policy=large"
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
