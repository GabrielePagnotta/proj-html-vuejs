<template>
    <div class="box">
        <ContentHeader :got="get"/>
    </div>
</template>

<script>
import ContentHeader from "../header/ContentHeader.vue"
    export default {
        name:"HeaderBox",
        components:{
            ContentHeader,
        },
        props:{
            get: Array
        },
        
        Data(){
            return{
                
            }
        }
    }
</script>

<style lang="scss" scoped>
.box{
    width:100%;
    height: 850px;
    background-image: url('../../assets/img/home_slider.jpg');
    background-size:cover;
    background-repeat: no-repeat;
}

.flex{
    display: flex;
}


</style>