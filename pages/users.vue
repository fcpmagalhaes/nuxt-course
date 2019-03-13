<template>
  <div>
    <input type="text" v-model="userId">
    <button @click="onLoaduser">Load User</button>
    <nuxt-child/>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userId: ""
    };
  },
  methods: {
    onLoaduser() {
      this.$router.push("/users/" + this.userId);
    }
  },
  layout: "users"
};
</script>
<style scoped>
</style>
