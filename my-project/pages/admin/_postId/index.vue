<template>
  <div class="admin-post-page">
    <section class="update-form">
      <admin-post-form :post="loadedPost"></admin-post-form>
    </section>
  </div>
</template>

<script>
import AdminPostForm from "@/components/Admin/AdminPostForm.vue";

export default {
  layout: 'admin',
  components: {
    AdminPostForm
  },
  data() {
      return {
          loadedPost: {
              author: 'Artdvp',
              title: 'My awesome Post',
              content: 'Super amazing, thanks for that!',
              thumbnailLink: 'https://www.articlesplanet.info/wp-content/uploads/2018/05/Tech-sector.jpg'
          }
      }
  }
};
</script>

<style scoped>
.update-form {
    width: 90%;
    margin: 20px auto;
}

@media (min-width: 768px) {
    .update-form {
        width: 500px;
    }
}
</style>
