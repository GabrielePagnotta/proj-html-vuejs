<template>
    <div class="main">
        <div class="flex">
            <div class="title-position">
                <h1>Live Dates</h1>
            </div>
            <div class="underline"></div>
            <article class="text">
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Sunt, iure eum sint nulla enim aperiam,
                    perferendis voluptate facilis cupiditate ipsam! Aliquam quibusdam obcaecati totam aperiam?</p>
            </article>
        </div>
        <DatesComponents />
    </div>
</template>

<script>
import DatesComponents from "./DatesComponents.vue"
export default {
    name: "DefaultTitle2",
    components:{
        DatesComponents,
    }
}
</script>

<style lang="scss" scoped>
.flex {
    display: flex;
    align-items: center;
    flex-direction: column;
}

h1 {
    font-size: 5.3rem;
    color: white;
}

.main {
    width: 100%;
    background-color: #252A33;
}

.title-position {
    margin-top: 70px;
}

.underline {
    width: 25%;
    height: 2px;
    background-color: #444E62;
    margin: 20px;
}

.text {
    font-size: 1.3rem;
    width: 50%;
    text-align: center;
    color: #7D7B8D;
    margin-top: 60px;
    margin-bottom: 100px;
}
</style>