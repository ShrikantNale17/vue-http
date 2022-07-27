<template>
  <!-- <CreatePost /> -->
  <!-- <PostList /> -->
  <!-- <ParentComp /> -->

  <TemplateRef />
</template>

<script>
// import PostList from "./components/PostList.vue";
// import CreatePost from "./components/CreatePost.vue";
// import ParentComp from "./components/ParentComp.vue";
import TemplateRef from "./components/TemplateRef.vue";

export default {
  name: "App",
  components: {
    // PostList,
    // CreatePost,
    // ParentComp,
    TemplateRef,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
