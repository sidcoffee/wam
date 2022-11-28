<template>
<!-- <div class="text-center"><img src="https://wellandtrulystuck.co.uk/wp-content/uploads/imported/Wham-Sticker-Cartoon-Batman-Style-Self-Adhesive-201498658126.JPG" width="200"/></div> -->
<div class="container p-0 m-0">
    <div id="timeline">GAME OVER</div>

    <div class="row m-0 p-0">
    <Wamboxsmall wamspeed='21s' @add-score="$emit('add-score', 1)"/>
    <Wamboxsmall wamspeed='11s' @add-score="$emit('add-score', 1)"/>
    <Wamboxsmall wamspeed='19s' @add-score="$emit('add-score', 1)"/>
    <Wamboxsmall wamspeed='9s' @add-score="$emit('add-score', 1)"/>
    </div>
    <div class="row m-0 p-0">
    <Wamboxsmall wamspeed='4s' @add-score="$emit('add-score', 1)"/>
    <Wamboxsmall wamspeed='13s' @add-score="$emit('add-score', 1)"/>
    <Wamboxsmall wamspeed='15s' @add-score="$emit('add-score', 1)"/>
    <Wamboxsmall wamspeed='25s' @add-score="$emit('add-score', 1)"/>

    </div>
    <div class="row m-0 p-0 d-none d-md-flex">
    <Wamboxsmall wamspeed='7s' @add-score="$emit('add-score', 1)"/>
    <Wamboxsmall wamspeed='2s' @add-score="$emit('add-score', 1)"/>
    <Wamboxsmall wamspeed='23s' @add-score="$emit('add-score', 1)"/>
    <Wamboxsmall wamspeed='17s' @add-score="$emit('add-score', 1)"/>

    </div>
   

</div>

</template>

<script>
import Wamboxsmall from "./Wamboxsmall.vue"

export default{
    name:'Wamboxbig',
    components:{
        Wamboxsmall,
    }
}
</script>

<style>
.container{
    max-width:1002px;
    z-index:99;
    cursor:url(cursor.cur), grab;

}
@keyframes timeline{
    from{width: 650px;};
    to{width: 0px;}

    0%{background:blue}
    70%{background:red}
}
#timeline:after{
    content:"";
    width:0px;
    height:5px;
    position: absolute;
    top:0;
    animation-name:timeline;
    animation-duration: 29s;
}
@keyframes gameover{
    0%{color:white;}
    80%{color:white}
    100%{color:red;}
}
#timeline{
    color:red;
    font-size:xx-large;
    font-weight: 700;
    animation-name:gameover;
    animation-duration:31s;
    }
   
</style>


Blackjack logic


062-123 10711363	carpark

call nab
eufy
doorbell

