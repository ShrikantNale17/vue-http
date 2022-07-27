<template>
  <div>
    <h4>Child Component</h4>
  </div>
</template>

<script>
export default {
  name: "ChildComp",
  beforeCreate() {
    console.log("beforeCreate child");
  },
  created() {
    console.log("created child");
  },
  beforeMount() {
    console.log("beforeMount child");
  },
  mounted() {
    console.log("mounted child");
  },
  beforeUpdate() {
    console.log("beforeUpdate child");
  },
  updated() {
    console.log("updated child");
  },
  beforeUnmount() {
    console.log("beforeUnmount child");
  },
  unmounted() {
    console.log("unmounted child");
  },
};
</script>

<style scoped></style>
