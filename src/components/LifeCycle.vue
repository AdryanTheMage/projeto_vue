<template>
<h1> Meu nome é: {{ nome }}</h1>
</template>
<script>
export default{
    name: 'LifeCycle',
    data(){return{
        nome:"Ainda Nao sei"

    }
},
created(){
    setTimeout(() =>{
    this.nome="Adryan"
    }, 1000);
},
mounted(){
     setTimeout(() =>{
    this.nome="fulipe meguil"
    }, 2000);
  
}
}
</script>