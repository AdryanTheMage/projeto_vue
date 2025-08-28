<template>
<img v-bind:src="avatar" :alt="descricao">

<MudarImagem @mudar-imagem="trocarImagem"/>
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
       
    },
    methods:{
        trocarImagem(){
            this.avatar= "/img/avatar2.jpg"
        }
    }
}

</script>