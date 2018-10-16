<template>
  <div class="editor flex col">
    <div class="topbar flex col">
      <p>top bar</p>
    </div>
    <div class="content">
      <text-block />
    </div>
  </div>
</template>

<script>
import TextBlock from "@/components/blocks/TextBlock.vue";

export default {
  components: { TextBlock }
};
</script>

<style lang="scss">
.editor {
  flex: 1;
  align-items: stretch;
}

.topbar {
  align-items: center;
  background-color: darkgrey;
}
</style>
