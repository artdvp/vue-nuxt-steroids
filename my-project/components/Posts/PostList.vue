<template>
    <section class="post-list">
      <post-preview id="1" :is-admin="isAdmin" thumbnail="https://www.articlesplanet.info/wp-content/uploads/2018/05/Tech-sector.jpg" title="Hello there!"
        previewText="This my first post!"></post-preview>
      <post-preview id="2" :is-admin="isAdmin" thumbnail="https://www.articlesplanet.info/wp-content/uploads/2018/05/Tech-sector.jpg" title="Hello !"
        previewText="This my second post!"></post-preview>
      <post-preview id="3" :is-admin="isAdmin" thumbnail="https://www.articlesplanet.info/wp-content/uploads/2018/05/Tech-sector.jpg" title="Hi!"
        previewText="This my third post!"></post-preview>
    </section>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview.vue'

export default {
  components: {
    PostPreview
  },
  props: {
    isAdmin: {
      type: Boolean,
      default: false  
    }
  }
}
</script>

<style scoped>
.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
