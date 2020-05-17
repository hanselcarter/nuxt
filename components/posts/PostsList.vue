<template>
  <div class="posts-page">
    <section class="posts">
      <PostPreview id="1" title="sometitle" previewText="lorem ipsum" />
      <PostPreview id="2" title="sometitle" previewText="lorem ipsum" />
    </section>
  </div>
</template>

<script>
import PostPreview from "@/components/posts/PostPreview";
export default {
  components: {
    PostPreview
  }
};
</script>

<style scoped>
.posts-page {
  display: flex;
  justify-content: center;
  align-items: center;
}
.posts-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>