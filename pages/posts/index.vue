<template>
  <div>
    <b-container>
      <h3>My Post Content</h3>
      <Header></Header>
      <PostContent></PostContent>
    </b-container>
  </div>
</template>

<script>
import Header from '@/components/posts/Header.vue'
import PostContent from '@/components/posts/PostContent.vue'

export default {
  components: {
    Header,
    PostContent,
  },
}
</script>

<style></style>
