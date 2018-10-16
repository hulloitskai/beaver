<template>
  <div id="app">
    <beaver />
  </div>
</template>

<script>
import Beaver from "@/components/Beaver.vue";
export default {
  components: { Beaver }
};
</script>

<style lang="scss">
body {
  margin: 0;

  font-family: "K2D", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

// prettier-ignore
p, h1, h2, h3, h4, h5, h6 {
  margin: 0;
}

// prettier-ignore
#app {
  position: absolute;
  left: 0; right: 0; top: 0; bottom: 0;
}
</style>
