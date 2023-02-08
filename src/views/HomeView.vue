<template>
  <div class="home">
  <Content :mode="mode" />
   
  </div>
</template>

<script>
// @ is an alias to /src
import Content from '@/components/Content.vue'

export default {
  name: 'HomeView',
  props: ['mode'],
  components: {
    Content,
  }
}
</script>
