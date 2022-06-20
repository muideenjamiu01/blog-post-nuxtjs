<template>
  <section class="post-list">
    <PostPreview
      id="1"
      :is-admin="isAdmin"
      thumbnail="https://video.cgtn.com/news/2021-01-16/Tech-It-Out-Chinese-tech-make-splashes-at-first-ever-virtual-CES-X6yZBqdwI0/video/10ed211d209541b5aec5cdf5129fea9b/10ed211d209541b5aec5cdf5129fea9b.jpg"
      title="Hello there!"
      previewText="This my first post!" />
    <PostPreview
      id="2"
      :is-admin="isAdmin"
      thumbnail="https://video.cgtn.com/news/2021-01-16/Tech-It-Out-Chinese-tech-make-splashes-at-first-ever-virtual-CES-X6yZBqdwI0/video/10ed211d209541b5aec5cdf5129fea9b/10ed211d209541b5aec5cdf5129fea9b.jpg"
      title="Hello there - the second time!"
      previewText="This my second post!" />
    <PostPreview
      id="3"
      :is-admin="isAdmin"
      thumbnail="https://video.cgtn.com/news/2021-01-16/Tech-It-Out-Chinese-tech-make-splashes-at-first-ever-virtual-CES-X6yZBqdwI0/video/10ed211d209541b5aec5cdf5129fea9b/10ed211d209541b5aec5cdf5129fea9b.jpg"
      title="Hi!"
      previewText="This my third post!" />
  </section>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'

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

