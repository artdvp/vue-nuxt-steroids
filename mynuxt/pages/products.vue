<template>
    <div>
        <h1 class="title">This is Products page</h1>
        <input type="text" v-model="pid">
        <button @click="onLoadProduct">Load Products</button>
        <nuxt-child />
    </div>
</template>

<script>
export default {
  data() {
    return {
      pid: ""
    };
  },
  methods: {
    onLoadProduct() {
      this.$router.push("/products/" + this.pid);
    }
  }
};
</script>