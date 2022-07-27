<template>
  <!-- <CreatePost /> -->
  <!-- <PostList /> -->
  <!-- <ParentComp /> -->

  <!-- <TemplateRef /> -->

  <ClickCounter />
  <HoverCounter />
</template>

<script>
// import PostList from "./components/PostList.vue";
// import CreatePost from "./components/CreatePost.vue";
// import ParentComp from "./components/ParentComp.vue";
// import TemplateRef from "./components/TemplateRef.vue";
import ClickCounter from "./components/ClickCounter.vue";
import HoverCounter from "./components/HoverCounter.vue";

export default {
  name: "App",
  components: {
    // PostList,
    // CreatePost,
    // ParentComp,
    // TemplateRef,
    ClickCounter,
    HoverCounter,
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
