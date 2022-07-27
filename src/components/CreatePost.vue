<template>
  <div>
    <form @submit.prevent="createPost">
      <div>
        <label for="title">Title : </label>
        <input type="text" id="title" v-model="formData.title" />
      </div>
      <div>
        <label for="body">Body : </label>
        <input type="text" id="body" v-model="formData.body" />
      </div>
      <div>
        <label for="userId">UserId : </label>
        <input type="text" id="userId" v-model="formData.userId" />
      </div>
      <button>Add Post</button>
    </form>
  </div>
</template>

<script>
import axios from "axios";

export default {
  name: "CreatePost",
  data() {
    return {
      formData: {
        title: "",
        body: "",
        userId: null,
      },
    };
  },
  methods: {
    createPost() {
      axios
        .post(`https://jsonplaceholder.typicode.com/posts`, this.formData)
        .then((res) => {
          console.log(res);
        })
        .catch((err) => {
          console.log(err);
        });
    },
  },
};
</script>

<style scoped></style>
