<template>
  <div class="admin-page">
    <section class="new-post" @click="$router.push('/admin/new-post')">
      <button class>create post</button>
    </section>
    <section class="existing-posts">
      <h1>Existing posts</h1>
      <PostsList isAdmin />
    </section>
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
.admin-page {
  padding: 20px;
}

.new-post {
  text-align: center;
  border-bottom: 2px solid #ccc;
  padding-bottom: 10px;
}

.existing-posts h1 {
  text-align: center;
}
</style>