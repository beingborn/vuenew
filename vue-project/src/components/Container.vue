<template>
  <div>
    <Post :PostData ='PostData[i]' v-for="(post,i) in PostData" :key="i"/>
  </div>
</template>

<script>

import Post from './Post.vue'

export default {
  name: 'Container',
  components : {
    Post : Post
  },
  props: {
    PostData : Array,
  },
}
</script>

<style>

</style>