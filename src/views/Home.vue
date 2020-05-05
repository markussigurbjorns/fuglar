<template>
  <div class="home">
    <bird-list />
  </div>
</template>

<script lang="ts">
// @ is an alias to /src
import BirdList from '@/components/BirdList.vue'

export default {
  name: 'Home',
  components: {
    BirdList
  }
}
</script>

<style scoped>

   

</style>
