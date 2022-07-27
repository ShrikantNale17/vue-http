<template>
  <div>
    <h4>Parent Component</h4>
    <button @click="showChild = !showChild">
      {{ showChild ? "Hide" : "Show" }} Child
    </button>
    <child-comp v-if="showChild" />
  </div>
</template>

<script>
import ChildComp from "./ChildComp.vue";

export default {
  name: "ParentComp",
  components: {
    ChildComp,
  },
  data() {
    return {
      showChild: true,
    };
  },
  beforeCreate() {
    console.log("beforeCreate parent");
  },
  created() {
    console.log("created parent");
  },
  beforeMount() {
    console.log("beforeMount parent");
  },
  mounted() {
    console.log("mounted parent");
  },
  beforeUpdate() {
    console.log("beforeUpdate parent");
  },
  updated() {
    console.log("updated parent");
  },
  beforeUnmount() {
    console.log("beforeUnmount parent");
  },
  unmounted() {
    console.log("unmounted parent");
  },
};
</script>

<style scoped></style>
