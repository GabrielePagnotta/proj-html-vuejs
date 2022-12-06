<template>
    <div class="padding">
        <div class="tab">
        <input type="checkbox" id="chck1">
        <label class="tab-label" for="chck1">17/08/2020 GEM FESTIVAL 2020 ANAKALIA, GEORGIA</label>
        <div class="tab-content dflex">
          <div>
            <img src="../../assets/img/maps.png" alt="">
          </div>
          <div>
            <h5>Untold stories</h5>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus voluptatem molestiae consequatur natus, reiciendis cumque eos necessitatibus! Alias a dolorum corporis, ratione vitae, odit iure ex, asperiores optio enim corrupti.</p>
            <button>BOOK NOW</button>
          </div>
        </div>
      </div>

      <div class="tab">
        <input type="checkbox" id="chck2">
        <label class="tab-label" for="chck2">24/9/2020 GROOVEFEST DOMINICAL REPUBLIC</label>
        <div class="tab-content dflex">
          <div>
            <img src="../../assets/img/maps.png" alt="">
          </div>
          <div>
            <h5>Untold stories</h5>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus voluptatem molestiae consequatur natus, reiciendis cumque eos necessitatibus! Alias a dolorum corporis, ratione vitae, odit iure ex, asperiores optio enim corrupti.</p>
            <button>BOOK NOW</button>
          </div>
        </div>
      </div>

      <div class="tab">
        <input type="checkbox" id="chck3">
        <label class="tab-label" for="chck3">31/10/2020 OASIS FESTIVAL 2020 MARRAKECH, MOROCCO</label>
        <div class="tab-content dflex">
          <div>
            <img src="../../assets/img/maps.png" alt="">
          </div>
          <div>
            <h5>Untold stories</h5>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus voluptatem molestiae consequatur natus, reiciendis cumque eos necessitatibus! Alias a dolorum corporis, ratione vitae, odit iure ex, asperiores optio enim corrupti.</p>
            <button>BOOK NOW</button>
          </div>
        </div>
      </div>

      <div class="tab">
        <input type="checkbox" id="chck4">
        <label class="tab-label" for="chck4">07/11/2020 MOGA FEESTIVAL - ESSAOURIAL, MOROCCO</label>
        <div class="tab-content dflex">
          <div>
            <img src="../../assets/img/maps.png" alt="">
          </div>
          <div>
            <h5>Untold stories</h5>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus voluptatem molestiae consequatur natus, reiciendis cumque eos necessitatibus! Alias a dolorum corporis, ratione vitae, odit iure ex, asperiores optio enim corrupti.</p>
            <button>BOOK NOW</button>
          </div>
        </div>
      </div>

      <div class="tab">
        <input type="checkbox" id="chck5">
        <label class="tab-label" for="chck5">10/12/2020 ENVISION FESTIVAL - UVITA, COSTA RICA</label>
        <div class="tab-content dflex">
          <div>
            <img src="../../assets/img/maps.png" alt="">
          </div>
          <div>
            <h5>Untold stories</h5>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus voluptatem molestiae consequatur natus, reiciendis cumque eos necessitatibus! Alias a dolorum corporis, ratione vitae, odit iure ex, asperiores optio enim corrupti.</p>
            <button>BOOK NOW</button>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
    export default {
        name:"DatesComponents"
    }
</script>

<style lang="scss" scoped>
    .main{
        width:60%;
        margin: 0 auto;
    }

$midnight: #292d39;
$background : #323844;
// General

h1 {
  margin: 0;
  line-height: 2;
  text-align: center;
}
h2 {
  margin: 0 0 .5em;
  font-weight: normal;
}
input {
  position: absolute;
  opacity: 0;
  z-index: -1;
}

.padding{
  padding:3rem;
}
// Layout
.row {
  display:flex;
  .col {
    flex:1;
    &:last-child {
      margin-left: 1em;
    }
  }
}
/* Accordion styles */
.tabs {
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 4px 4px -2px rgba(0,0,0,0.5);
}
.tab {
  width: 60%;
  margin: 0 auto;
  margin-top: 10px;
  color: #ea4a56;
  overflow: hidden;
  font-size: 1.2rem;
  position: relative;
  z-index: 0;
  &-label {
    display: flex;
    padding: 1rem;
    background: $background;
    font-weight: bold;
    cursor: pointer;
    /* Icon */
    &:hover {
      background: darken($background, 10%);
    }
    &::before {
      content: "+";
      width: 1em;
      height: 1em;
      text-align: center;
      transition: all .35s;
      margin: 0 20px;
      color: #ea4a56;
    }
  }
  &-content {
    max-height: 0;
    padding: 0 1em;
    color: $midnight;
    background: $background;
    transition: all .35s;
  }
  &-close {
    display: flex;
    justify-content: flex-end;
    padding: 1em;
    font-size: 0.75em;
    background: $midnight;
    cursor: pointer;
    &:hover {
      background: darken($midnight, 10%);
    }
  }
  p{
    color: #7780a4;
    font-size: 1.2rem;
    margin-left: 1rem;
  }

  h5{
    color: white;
    margin-left:1rem;
    margin-bottom: 0.8rem;
    font-size: 1.4rem;
  }
  .dflex{
    display: flex;
    flex-direction: row;
    
}
 img{
    width: 100%;
}

button{
    background-color: #ea4a56;
    border: none;
    font-size: 1.5rem;
    margin: 1rem;
    color: white;
    padding: 10px;
}
}

// :checked
input:checked {
  + .tab-label {
    background: darken($midnight, 10%);
    &::before {
        content:"-";
        color: white;
      background-color:#ea4a56;
    }
  }
  ~ .tab-content {
    max-height: 100vh;
    padding: 1em;
  }

}

</style>