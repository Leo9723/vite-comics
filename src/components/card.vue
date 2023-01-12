<script>
export default {
  props: {
    img:String,
    title:String
  }
}
</script>
<template lang="">
    <div class="cardContainer">
        <div class="card">
            <img :src="img" alt="">
            <div>{{ title }}</div>
        </div>
    </div>
</template>
<style lang="scss">
   .cardContainer{
    width: calc(100% / 6);
    .card{
        margin-bottom: 20px;
        div{
             font-weight: bold;
             font-size: large;        
        }
    }
   }
</style>