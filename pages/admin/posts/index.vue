<template>
  
    <PostList isAdmin :posts="loadData" />
 
</template>
<script>
import PostList from '@/components/posts/PostList'
import axios from 'axios'
export default {
  layout: 'coreLayout',
  components: {
    PostList
  },
  computed: {
    loadData() {
      return this.$store.getters.getAllPosts
    }
  }
}
</script>