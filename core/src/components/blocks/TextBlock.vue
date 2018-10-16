<template>
  <div
    class="text block" :class="{ editing }"
    @click="handleClick"
  >
    <textarea
      class="content editing"
      ref="textarea"
      v-if="editing"
      v-model="content"
      @blur="handleBlur"
    />
    <p
      class="content viewing"
      v-else
    >
      {{ content }}
    </p>
  </div>
</template>

<script>
export default {
  data: function() {
    return { content: "", editing: false };
  },
  methods: {
    handleClick: function() {
      this.editing = true;
      this.$nextTick(() => this.$refs.textarea.focus());
    },
    handleBlur: function() {
      this.editing = false;
    }
  }
};
</script>

<style lang="scss" scoped>
.text.block {
  padding: 25px;
  background-color: rgb(206, 206, 206);
}
</style>
