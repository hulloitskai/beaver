<template>
  <div class="beaver flex">
    <div class="sidebar">
      <p>sidebar</p>
    </div>
    <editor />
  </div>
</template>

<script>
import Editor from "./Editor.vue";
export default {
  components: { Editor }
};
</script>

<style lang="scss">
// prettier-ignore
.beaver {
  // Fullscreen self in parent window.
  width: 100%;
  height: 100%;

  align-items: stretch;
}

// prettier-ignore
.flex { display: flex; }
// prettier-ignore
.col { flex-direction: column; }
</style>
