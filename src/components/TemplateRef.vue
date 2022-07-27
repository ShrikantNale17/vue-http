<template>
  <div>
    <input type="text" ref="inputRef" />
  </div>
  <PostList ref="childRef" />
</template>

<script>
import PostList from "./PostList.vue";

export default {
  name: "TemplateRef",
  mounted() {
    console.log(this.$refs.childRef);
    this.$refs.inputRef.focus();
  },
  components: {
    PostList,
  },
};
</script>

<style scoped></style>
