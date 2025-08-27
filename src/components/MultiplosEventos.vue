<template>
<div>
    <button @click="Primeiro($event),segundo($evento)">Ativar múltiolos eventos</button>
    <p>{{ multiplos_eventos }}</p>
</div>
</template>
<script>
import PrimeiroComponente from './PrimeiroComponente.vue';

export default{
    name:'MultiplosEventos',
    data(){
return{
    multiplos_eventos:""
}
    },
    methods:{
        Primeiro(e){
            this.multiplos_eventos="Primeiro evento ativado"
            
        },
        segundo(e){
        setTimeout(()=> this.multiplos_eventos = "Segundo Evento",500)
        }
    }

    
}
</script>
<style scoped>
div{
    margin: 100px;
}</style>