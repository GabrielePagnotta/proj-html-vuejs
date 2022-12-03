<template>
    <div class="main-container dflex main-gap">
        <div>
            <div class="img-horizontal bg-mixer dflex">
                <div class="description h-des-horizontal">
                   <h1>Tecnology and music</h1> 
                   <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, recusandae?</p>
                </div>
            </div>
            <div class="vertical-content-cards main-gap dflex">
                <div class=" bg-guitars dflex flex-end">
                <div class="description">
                   <h1>Tecnology and music</h1> 
                   <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, recusandae?</p>
                </div>
                </div>

                <div class="bg-folders dflex flex-end">
                    <div class="description">
                   <h1>Tecnology and music</h1> 
                   <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, recusandae?</p>
                </div>
                </div>
            </div>
            <div class="img-horizontal bg-public dflex">
                <div class="description h-des-horizontal">
                   <h1>The flavor of rock</h1> 
                   <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, recusandae?</p>
                </div>
            </div>
        </div>
        <div class="dflex main-gap f-col">
            <div class="grid-2-cards bg-car dflex">
                <div class="description">
                    <h1>Taking it back to the old school</h1>
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quo, explicabo!</p>
                </div>
            </div>

            <div class="grid-2-cards bg-composer dflex">
                <div class="description h-des-guitar">
                    <h1>Taking it back to the old school</h1>
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quo, explicabo!</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name:"GridContent",
    }
</script>

<style lang="scss" scoped>

// FLEX COMPOSITION
.main-gap{
    gap:20px
}
.dflex{
    display: flex;
}
.jc-center{
    justify-content:center;
}


.flex-end{
    align-items: flex-end;
}

.f-col{
    flex-direction: column;
}

.main-gap{
    gap:20px;
}
// ---------------------------------------------------

// CONTAINERS
.main-container{
    width:60%;
    margin:0 auto;
}

.vertical-content-cards{
    width: 100%;
    height: 600px;
    
}
.grid-2-cards{
    width: 100%;
    height:calc(100% / 2);
    background-size: cover;
    background-repeat: no-repeat;
    align-items: flex-end;
    
}

.img-horizontal{
    width: 100%;
    height:350px;
    background-size: cover;
    align-items: flex-end;
}

.description{
    width: 100%;
    height:30%;
    background-color: #313141;
    color: #626984;
    
}
.h-des-guitar{
    height:27%;
}

.h-des-horizontal{
    height:40%;
}
// -------------------------------------------------------
// BACKGROUND IMAGES
.bg-folders{
    background-image: url(../../assets/img/blog-post4.jpg);
    background-size: cover;
}

.bg-guitars{
    background-image: url(../../assets/img/blog-post3.jpg);
    background-size: cover;
}

.bg-mixer{
    background-image: url(../../assets/img/blog_music_techo-800x400.jpg);
    background-size: cover;
}

.bg-public{
background-image:url(../../assets/img/blog_flavor_rock.jpg);
}

.bg-car{
    background-image:url(../../assets/img/blog-post1.jpg);
    background-size: cover;
}

.bg-composer{
    background-image:url(../../assets/img/blog-post2.jpg);
    background-size: cover;
}
// -----------------------------------------------------------------------------
// STATICS TAGS CONFIGS
h1{
    color: #ea4a56;
    margin: 10px 20px;
    font-size: 1.4rem;
}

p{
    font-size: 1.2rem;
    margin:10px 25px;
    line-height: 30px;
}
// ---------------------------------------------------------------------------------




</style>