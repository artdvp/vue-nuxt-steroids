<template>
  <div class="posts-page">
    <post-list :posts="loadedPosts"></post-list>
  </div>
</template>

<script>
import PostList from "@/components/Posts/PostList.vue";

export default {
  components: {
    PostList
  },
  asyncData(context, callback) {
    setTimeout(() => {
      callback(null, {
        loadedPosts: [
          {
            id: "1",
            title: "First Post",
            previewText: "This is our first post!",
            thumbnail:
              "https://www.articlesplanet.info/wp-content/uploads/2018/05/Tech-sector.jpg"
          },
          {
            id: "2",
            title: "Second Post",
            previewText: "This is our second post!",
            thumbnail:
              "https://www.articlesplanet.info/wp-content/uploads/2018/05/Tech-sector.jpg"
          }
        ]
      });
    }, 1500);
  }
};
</script>

<style scoped>
.posts-page {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
