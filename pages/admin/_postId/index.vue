<template>
  <div class="admin-post-page">
    <section class="update-form">
      <AdminPostForm :post="loadedPost" />
    </section>
  </div>
</template>

<script>
import AdminPostForm from "@/components/admin/AdminPostForm";

export default {
  components: { AdminPostForm },
  data() {
    return {
      loadedPost: {
        author: "some",
        title: "somethign",
        content: "ssr",
        thumbnailLink:
          "https://images.pexels.com/photos/1105666/pexels-photo-1105666.jpeg?cs=srgb&dl=people-at-concert-1105666.jpg&fm=jpg"
      }
    };
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