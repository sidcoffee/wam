<template>
<div class="round">
    <Wombat :wamspeedthree = 'wamspeedtwo' @add-score="$emit('add-score', 1)" />
</div>
</template>

<script>
import Wombat from "./Wombat.vue"
export default{
    name:'Round',
    data(){
        return{
        }
    },
    components:{
        Wombat,
    },
    props:{
        wamspeedtwo:String,
    },
    methods:{

    }
}
</script>

<style scoped>
.round{
    width:140px;
    height:140px;
    border:1px solid red;
    border-radius:100px;
    background:#fff;
    margin:22px auto;
    z-index:-2;
    overflow: hidden;
}
@media only screen and (max-width: 600px) {

.round{
width: 70px;
height: 70px;
}

}
</style>