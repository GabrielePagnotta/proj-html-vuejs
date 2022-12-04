<template>
    <div class="citation-box dflex">
        <p>"I just listened to it and said to myself,"Man, i really love this album." Still, today, it just sounds so fresh. It sounds full of ideas. These guys knew what they were doing. They're good, And they're inventive. I haven't heard anything this year that's as inventive. I don't really expect to."</p>
        <font-awesome-icon icon="fa-solid fa-play" />
    </div>
</template>

<script>
    export default {
        name:"CitationContent",
    }
</script>

<style lang="scss" scoped>
    .citation-box{
        width: 42%;
        height: 500px;
        margin: 0 auto;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        
    }

    .dflex{
        display: flex;
    }

    .fa-play{
        color: white;
        background-color: #ea4a56;
        font-size: 1.6rem;
        padding: 30px;
        border-radius:100px;
        transition: background-color 0.5s, color 0.5s;
    }

    p{
        text-align: center;
        color: white;
        font-size: 1.4rem;
        margin:30px;
        line-height: 40px;
        font-style: italic;
    }

    .fa-play:hover{
        color: black;
        background-color: white;
    }
</style>