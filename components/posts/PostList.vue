<template>
 
    <b-row class="py-2">
      <PostContent
        v-for="post in posts"
        :key="post.id"
        :id="post.id"
        :title="post.title"
        :content="post.content"
        :image="post.image"
        :isAdmin="isAdmin"
      />
    </b-row>
  
</template>
<script>
import PostContent from '@/components/posts/PostContent'
export default {
  components: {
    PostContent
  },
  props: {
    isAdmin: {
      type: Boolean,
      default: false
    },
    posts: {
      type: Array,
      required: true
    }
  }
}
</script>
