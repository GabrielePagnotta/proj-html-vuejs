<template>
    <div class="main flex">
        <div class="line"></div>
        <div class="title-position">
            <h1>{{title}}</h1>
        </div>
        <div class="underline"></div>
        <article class="text">
            <p>{{subtitle}}</p>
        </article>
        
    </div>
</template>

<script>

    export default {
        name:"DefaultTitle",
        data(){
            return{
                title:"Music is life",
                subtitle:"Lorem ipsum, dolor sit amet consectetur adipisicing elit. Sunt, iure eum  sint nulla enim aperiam, perferendivoluptate facilis cupiditate ipsam! Aliquam quibusdam obcaecati totam aperiam?",
            }
        }
    }
</script>

<style lang="scss" scoped>
.flex{
    display: flex;
    align-items: center;
    flex-direction: column;
}

.line{
    width:25%;
    height: 15px;
    background-color: #ea4a56 ;
}
.main{
    width: 100%;
    background-color: #323844;
}

h1{
    font-size: 5.3rem;
    color: white;
}

.title-position{
    margin-top: 70px;
}

.text{
    font-size: 1.3rem;
    width: 50%;
    text-align: center;
    color: #7D7B8D;
    margin-top: 60px;
    margin-bottom: 100px;
}

.underline{
    width:23%;
    height:2px;
    background-color:#444E62;
    margin: 20px;
}

</style>