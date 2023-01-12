<script>
import AppList from './card.vue'

export default {
  components: {
    AppList
  },
  data(){
    return {
      
    }
  }
}
</script>
<template lang="">
  <div class="maincont">
    <AppList v-for="(card, index) in AppList" :img="card.thumb" :title="card.series">
  </div>
</template>
<style lang="scss">
   .maincont {
    padding: 50px;
    background-color: black;
    color: white;
    font-size: 70px;
   }
</style>
