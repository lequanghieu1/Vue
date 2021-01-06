<template>
  <login :acc="acc" />
  <router-view />
</template>

<script>
import login from "./components/Login.vue";

export default {
  name: "App",
  components: {
    login,
  },
  data() {
    return {
      acc: [
        { id: 1, username: "user1", pass: "123" },
        { id: 2, username: "user2", pass: "123" },
      ],
    };
  },
};
</script>

<style></style>
