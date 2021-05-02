<template>
	<section class="post-list">
    <PostPreview
      id="1"
      :isAdmin="isAdmin"
      thumbnail="https://res.cloudinary.com/people-matters/image/upload/q_auto,f_auto/v1578710070/1578710068.jpg"
      title="Hello There!"
      previewText="This is my first post!"
    />
    <PostPreview
      id="2"
      :isAdmin="isAdmin"
      thumbnail="https://res.cloudinary.com/people-matters/image/upload/q_auto,f_auto/v1578710070/1578710068.jpg"
      title="Hello There!"
      previewText="This is my second post!"
    />
    <PostPreview
      id="3"
      :isAdmin="isAdmin"
      thumbnail="https://res.cloudinary.com/people-matters/image/upload/q_auto,f_auto/v1578710070/1578710068.jpg"
      title="Hello There!"
      previewText="This is my third post!"
    />
    <PostPreview
      id="4"
      :isAdmin="isAdmin"
      thumbnail="https://res.cloudinary.com/people-matters/image/upload/q_auto,f_auto/v1578710070/1578710068.jpg"
      title="Hello There!"
      previewText="This is my fourth post!"
    />
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
.posts-pages {
  display: flex;
  justify-content: center;
  align-items: center;
}
.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>