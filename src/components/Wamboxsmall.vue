<template>
    <div class="box col-md-3 col-6 col-sm-6">
        <Round :wamspeedtwo='wamspeed' @add-score = "$emit('add-score', 1)" />

    </div>

</template>

<script>
import Round from "./Round.vue"
export default{
    name:'Wamboxsmall',
    components:{
        Round,
    },
    props:{
        wamspeed:String,
    },
    methods:{
        showwam(){
        }
    }
}
</script>

<style scoped>
.box{
    /* width:200px;
    height:200px; */
    border:1px solid red;
    z-index:1;
    overflow: hidden;
    background:url('https://mineblocks.com/1/wiki/images/archive/d/df/20211221200859%21Wood.png');
}
</style>