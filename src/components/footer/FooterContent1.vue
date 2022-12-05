<template>
<div>
    <section class="container bg-1">
        <div class="box1">
            <img src="../../assets/img/logo_footer.png" alt="footer-images">
        </div>
        <div class="box2">
            <ul>
                <li v-for="(element,index) in got" :key="index">
                    <a :href="element.link">{{element.name}}</a>
                </li>
            </ul>
        </div>
    </section>
    <section class="container bg-2">
        <div class="box1">
            <ul>
                <li>&copy;copyright 2012-2020</li>
                <li>|</li>
                <li>AVADA BY THEME FUSION</li>
                <li>|</li>
                <li>ALL RIGHTS RESERVED</li>
                <li>|</li>
                <li>POWERED BY MYSELF</li>
            </ul>
        </div>
        <div class="box2">
            <font-awesome-icon icon="fa-brands fa-facebook" />
            <font-awesome-icon icon="fa-brands fa-twitter" />
            <font-awesome-icon icon="fa-brands fa-instagram" />
            <font-awesome-icon icon="fa-brands fa-youtube" />
        </div>
    </section>
</div>
</template>

<script>
    export default {
        name:"FooterContent1",
        props:{
            got:Array,  
        },

    }
</script>

<style lang="scss" scoped>
.container{
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding:20px;
}

.fa-facebook{
    font-size: 1.6rem;
    margin:5px;
    background-color: #313141;
    color: white;
    padding: 10px;
    cursor: pointer;
    
}

.fa-twitter{
    font-size: 1.6rem;
    margin:5px;
    background-color: #313141;
    color: white;
    padding: 10px;
    cursor: pointer;
}

.fa-instagram{
    font-size: 1.6rem;
    margin:5px;
    background-color: #313141;
    color: white;
    padding: 10px;
    cursor: pointer;
}
.fa-youtube{
    font-size: 1.6rem;
    margin:5px;
    background-color: #313141;
    color: white;
    padding: 10px;
    cursor: pointer;
}

.fa-youtube:hover{
    color: black;
    background-color: white;
}

.fa-facebook:hover{
    color: black;
    background-color: white;
}

.fa-instagram:hover{
    color: black;
    background-color: white;
}

.fa-twitter:hover{
    color: black;
    background-color: white;
}


.bg-1{
    background-color: #313141;
}

.bg-2{
    background-color: #21212c;
    padding: 40px;
}
li a{
    float: left;
    margin: 10px;
    text-decoration: none;
    color: gray;
}

li{
    float:left;
    font-size: 15px;
    color: gray;
    cursor: pointer;
}


li:nth-child(even){
    margin:0 10px;
}

img{
    margin: 10px;
    cursor: pointer;
}

.box1{
    width: 65%;
   
}

.box2{
    width: 35%;
    display: flex;
    justify-content: end;
}


a:hover{
    color: white;
}

li:hover{
    color: white;
}
</style>