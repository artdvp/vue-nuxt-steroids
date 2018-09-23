<template>
  <section class="container">
    <Header/>
    <div>
      <nuxt-link to="/users">Users</nuxt-link>
      <br>
      <br>
      <button @click="goProduct">Go Product</button>
    </div>
  </section>
</template>

<script>
export default {
  methods: {
    goProduct() {
      this.$router.push('/products')
    }
  }
}
</script>

<style>
</style>
