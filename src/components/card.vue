<script>
export default {
    props: {
        img: String,
        title: String,
    }
}
</script>
<template lang="">
    <div>
        <img :src="img" alt="">
        <h4>{{ title }}</h4>
    </div>
</template>
<style lang="">
    
</style>