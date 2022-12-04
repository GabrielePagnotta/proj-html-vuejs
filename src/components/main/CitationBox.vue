<template>
    <div class="main">
        <CitationContent />
    </div>
</template>

<script>
import CitationContent from "./CitationContent.vue"
    export default {
        name:"CitationBox",
        components:{
            CitationContent,
        }
    }
</script>

<style lang="scss" scoped>
    .main{
        width: 100%;
        background-image: url(../../assets/img/home-testimonial-parallax.jpg);
        background-size: cover;
        padding: 100px;
    }
</style>