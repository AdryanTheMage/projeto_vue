<template>
  <Header/>
<h1>olá Mundo</h1>

<PrimeiroComponente/>
<LifeCycle/>
<Pessoa/>


</template>
<script>
import PrimeiroComponente  from './components/PrimeiroComponente.vue';
import LifeCycle from './components/LifeCycle.vue';
import Pessoa from './components/Pessoa.vue';
import Header from './components/Header.vue';

export default{
  name:'App',
  components:{
    PrimeiroComponente,
    LifeCycle,
    Pessoa,
Header
 
  }
}
</script>
<style>
body{
  background-color: rgb(0, 0, 0);
  color:rgb(87, 25, 25);

  a{
    color: rgb(255, 0, 0);
  
    }
    }
    
.teste
      {background-color:#fff
}
    </style>