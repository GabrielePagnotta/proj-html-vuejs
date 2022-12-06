<template>
    <div class="container dflex">
        <p>{{Buttonname}}</p>
    </div>
</template>

<script>
    export default {
        name:"ViewAllDates",
        data(){
            return{
                Buttonname:"VIEW ALL LIVE DATES"
            }
        }
    }
</script>

<style lang="scss" scoped>
    .container{
        width: 100%;
        height:100px;
        background-color:#ea4a56;
        color: white;
        transition: background-color 0.5s linear;
        word-spacing: 5px;
    }

    .dflex {
    display: flex;
    align-items: center;
    justify-content: center;
}

.container:hover{
    background-color: white;
    color: black;
    word-spacing: 5px;
}
</style>