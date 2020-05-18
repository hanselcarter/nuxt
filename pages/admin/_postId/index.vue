<template>
  <div class="admin-new-post-page">
    <section class="new-post-form">
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