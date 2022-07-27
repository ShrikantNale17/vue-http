<template>
  <div>
    <button @click="incrementCount">Clicked {{ count }} times</button>
  </div>
</template>

<script>
import CounterMixin from "../mixins/counter";

export default {
  name: "ClickCounter",
  data() {
    return {
      count: 100,
    };
  },
  mixins: [CounterMixin],
};
</script>

<style scoped></style>
