<template>
  <section class="container">
    <button @click="onLoadProducts">Products</button>
    <button @click="onLoadUsers">Users</button>
  </section>
</template>

<script>
export default {
  methods: {
    onLoadProducts() {
      this.$router.push("/products");
    },
    onLoadUsers() {
      this.$router.push("/users");
    }
  }
};
</script>