<template>
    <div class="main-container dflex main-gap">
        <div class="grid-1-cards main-gap dflex f-col">
            <div class="img-horizontal bg-mixer">
                <div class="bg-color">
                    <p class="text-position">Tecnology and music</p>
                </div>
                <div class="description h-des-horizontal">
                    <h1>Tecnology and music</h1>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, recusandae?</p>
                </div>
           </div>
            <div class="vertical-content-cards main-gap dflex">
                <div class="card bg-guitars ">
                    <div class="bg-color">
                        <p class="text-position-vertical">While my guitar gently deeps</p>
                    </div>
                    <div class="description-vertical">
                        <h1>While my guitar gently deeps</h1>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, recusandae?</p>
                    </div>
                </div>

                <div class="card bg-folders  flex-end">
                    <div class="bg-color">
                        <p class="text-position-vertical-2">it's just sound better</p>
                    </div>
                    <div class="description-vertical">
                        <h1>it's just sound better</h1>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, recusandae?</p>
                    </div>
                </div>
            </div>
            <div class="img-horizontal bg-public ">
                <div class="bg-color">
                    <p class="text-position">Tecnology and music</p>
                </div>
                <div class="description3 h-des-horizontal">
                    <h1>The flavor of rock</h1>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, recusandae?</p>
                </div>
            </div>
        </div>
        <div class="dflex main-gap f-col">
            
                <div class="img-vertical bg-car ">
                    <div class="bg-color">
                        <p class="text-position-vertical">Taking it back to the old school</p>
                    </div>
                    <div class="description-vertical">
                        <h1>Taking it back to the old school</h1>
                        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quo, explicabo!</p>
                    </div>
                </div>

                <div class="img-vertical bg-composer ">
                    <div class="bg-color">
                        <p class="text-position-vertical">Sharing the stage with a legend</p>
                    </div>
                    <div class="description4">
                        <h1>Sharing the stage with a legend</h1>
                        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quo, explicabo!</p>
                    </div>

                </div>
                
        </div>
    </div>
</template>

<script>
export default {
    name: "GridContent",
}
</script>

<style lang="scss" scoped>
// FLEX COMPOSITION
.main-gap {
    gap: 20px
}

.dflex {
    display: flex;
}

.jc-center {
    justify-content: center;
}

.al-center{
    align-items: center;
}

.flex-end {
    align-items: flex-end;
}

.f-col {
    flex-direction: column;
}

.main-gap {
    gap: 20px;
}

// ---------------------------------------------------

// CONTAINERS
.main-container {
    width: 60%;
    margin: 0 auto;
}

.vertical-content-cards {
    width: 100%;
    height: 600px;

}

.grid-2-cards {
    width: 100%;
    height: calc(100% / 2);
    align-items: flex-end;
    transition: transform 1s;
}

.grid-1-cards {
    width: 100%;
    height: calc(100% / 3);
    align-items: flex-end;

}

.img-horizontal {
    width: 100%;
    height: 350px;
    align-items: flex-end;
    transition: transform 1s;
    
    
}

.img-vertical {
    width: 100%;
    height: 100%;
    align-items: flex-end;
    transition: transform 1s;
    
}

.card{
    transition: transform 1s;
}


.description {
    visibility: visible;
    width: 100%;
    height: 30%;
    background-color: #313141;
    color: #626984;
    transition: visibility 0.5s, opacity 0.5s;
    position: relative;
    z-index: 1;
    top: -42%;

}

.description3 {
    visibility: visible;
    width: 100%;
    height: 30%;
    background-color: #313141;
    color: #626984;
    transition: visibility 0.5s, opacity 0.5s;
    position: relative;
    z-index: 1;
    top: -43%;

}

.description4 {
    visibility: visible;
    width: 100%;
    height: 30%;
    background-color: #313141;
    color: #626984;
    transition: visibility 0.5s, opacity 0.5s;
    position: relative;
    z-index: 1;
    top: -31.5%;

}
.description-vertical {
    visibility: visible;
    width: 100%;
    height: 30%;
    background-color: #313141;
    color: #626984;
    transition: visibility 0.5s, opacity 0.5s;
    position: relative;
    top: -31%;

}

.h-des-guitar {
    height: 27%;
}

.h-des-horizontal {
    height: 40%;
}

.bg-color{
    visibility: visible;
    opacity: 0;
    width: 100%;
    height: 100%;
    background-color: #ea4a56;
    transition: visibility 0.7s linear,opacity 0.7s linear;
    position: relative;
    
    
}
.text-position{
    margin: 0;
    color: white;   
    position: relative;
    top: 50%;
    left: 35%;
}

.text-position-vertical{
    margin: 0;
    color: white;   
    position: relative;
    top: 40%;
    left: 15%;
}

.text-position-vertical-2{
    margin: 0;
    color: white;   
    position: relative;
    top: 40%;
    left: 25%;
}



// -------------------------------------------------------

// BACKGROUND IMAGES
.bg-folders {
    background-image: url(../../assets/img/blog-post4.jpg);
    background-size: cover;
}

.bg-guitars {
    background-image: url(../../assets/img/blog-post3.jpg);
    background-size: cover;
}

.bg-mixer {
    background-image: url(../../assets/img/blog_music_techo-800x400.jpg);
    background-size: cover;
}

.bg-public {
    background-image: url(../../assets/img/blog_flavor_rock.jpg);
}

.bg-car {
    background-image: url(../../assets/img/blog-post1.jpg);
    background-size: cover;
}

.bg-composer {
    background-image: url(../../assets/img/blog-post2.jpg);
    background-size: cover;
}



// -----------------------------------------------------------------------------

// STATICS TAGS CONFIGS
h1 {
    color: #ea4a56;
    margin: 10px 20px;
    font-size: 1.4rem;
}

p {
    font-size: 1.2rem;
    margin: 10px 25px;
    line-height: 30px;
}

.img-horizontal:hover{
    transform: scale(1.1);
    
}



.img-horizontal:hover .bg-color{
    display: block;
    visibility: visible;
    opacity: 0.8;
    
}

.img-horizontal:hover .description{
    visibility: hidden;
    opacity: 0;
}

.img-horizontal:hover .description3{
    visibility: hidden;
    opacity: 0;
}

.img-vertical:hover{
    transform: scale(1.1);
}

.img-vertical:hover .bg-color{
    display: block;
    visibility: visible;
    opacity: 0.8;
}

.img-vertical:hover .description-vertical{
    visibility: hidden;
    opacity: 0;
}

.img-vertical:hover .description4{
    visibility: hidden;
    opacity: 0;
}
.card:hover{
    transform: scale(1.1); 
}

.card:hover .bg-color{
    display: block;
    visibility: visible;
    opacity: 0.8;
}

.card:hover .description-vertical{
    visibility: hidden;
    opacity: 0;
}
// ---------------------------------------------------------------------------------
</style>