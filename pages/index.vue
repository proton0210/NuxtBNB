<template>
  <div>
    <div v-for="home in homes" :key="home">
      <h1>{{ home.title }}</h1>
      <br />
    </div>
  </div>
</template>

<script>
import homes from "~/data/homes.json";

export default {
  name: "IndexPage",
  data() {
    return {
      homes: homes.slice(0, 3),
    };
  },
};
</script>
