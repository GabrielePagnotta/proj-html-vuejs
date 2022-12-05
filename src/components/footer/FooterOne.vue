<template>
    <div>
        <FooterContent1 :image="img" :got="get"/>
    </div>
</template>

<script>
import FooterContent1 from "./FooterContent1.vue"
    export default {
        name:"FooterOne",
        components:{
            FooterContent1,
            
        },
        props:{
            get: Array,
            
        },
    }
</script>

<style lang="scss" scoped>

</style>