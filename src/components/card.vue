<script>
export default {
    props: {
        img: string,
        title: string,
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