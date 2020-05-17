<template>
  <div class="posts-page">
    <PostsList id="1" title="sometitle" previewText="lorem ipsum" />
  </div>
</template>

<script>
import PostsList from "@/components/posts/PostsList";
export default {
  components: {
    PostsList
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