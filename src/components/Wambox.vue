<template>
<Wamboxbig @add-score='countscore' />
<h1 class='p-5 text-center'>SCORE: <span style="color:red;font-size:xxx-large">{{count}}</span></h1>
</template>

<script>
import Wamboxbig from './Wamboxbig.vue';

export default{
    name:'Wambox',
    components:{
        Wamboxbig,
    },
    data(){
        return{
            count:0,
        }
    },
    methods:{
        countscore(score){
            this.count += score;
        }
    }
}
</script>

<style scoped>


</style>