<template>
<img v-bind:src="avatar" :alt="descricao">
<MudarImagem/>
</template>
<script>

import MudarImagem from './MudarImagem.vue';
export default{
    name:'Picture',
    components:{
        MudarImagem
    },
    
    data(){
        return{

            avatar: '/img/hq2.jpg',
            descricao:"Ai Ai bolsonaro (Kleberiano)"
        }
    }
}

</script>