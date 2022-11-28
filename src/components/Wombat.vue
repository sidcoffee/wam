<template>
    <img :src="images[index].src" :style="{animationDelay: wamspeedthree}" @click = "wammed()" id="womimg" :class="[wammy? 'wamboy':'']">
</template>

<script>
export default{
    name:'Wombat',
    data(){
        return{
            color:'',
            index:0,
            wammy:false,
            // score:0,
            images:[{
                src:'https://i.pinimg.com/originals/50/71/e1/5071e19e2d63f7e3b61921ecab0cc409.png'
            },
            {
                src:'https://cdn-icons-png.flaticon.com/256/6028/6028731.png'
            }
        ]
        }
    },
    props:{
        wamspeedthree:String,
    },
    methods:{

        wammed(){
            this.index = 1;
            this.wammy=true;
            // this.score = this.score+1;
            this.$emit('add-score', 1);

        
    },
    
},
    created(){

    },

}
</script>

<style scoped>
@keyframes gotop{
    0% {bottom: -225px;}
    25% {bottom:-100px;}
    50% {bottom:-125px;}
    75% {bottom:-150px}
    100%{bottom:-245px;}
    
}

@keyframes gotopmobile{
    0% {bottom: -65px;}
    25% {bottom:0px;}
    50% {bottom:-30px;}
    75% {bottom:-50px}
    100%{bottom:-75px;}
    
}

#womimg{
    width:150px;
    margin-left: 10px;
    margin-top: -35px;
    position: absolute;
    bottom: -245px;
    animation-name:gotop;
    animation-duration:1s;
    cursor:pointer;
    -webkit-user-drag: none;
    -khtml-user-drag: none;
    -moz-user-drag: none;
    -o-user-drag: none;
    user-drag: none;
}
@media only screen and (max-width: 600px) {

#womimg{
width: 75px;
height: 75px;
margin-left: 0;
margin-top: 0;
bottom: -75px;
animation-name:gotopmobile;
}

}
.wamboy{
    bottom:0!important;
    animation:none;
    right:-7px;
    pointer-events: none;
}
</style>


Consultations
Planning and Design
Development of the website (Beta Version)
UAT
Feedback, bugs
Updates and fixes
Launch


