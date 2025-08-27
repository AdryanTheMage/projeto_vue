<template>
    <div>
    <h2>Meu Formulário</h2>
    <form action=""@submit="enviarFormulario($event)">
        <div>
         <input type="texy" v-model="name">
         </div>
         <div>
           <InputText/>
           </div>
    <Submit/>
    </form>
   <p>Conteúdo</p>
   <p>Conteúdo</p>
   <p>Conteúdo</p>
    </div>
</template>

<script>
import InputText from './form/InputText.vue';

import Submit from './form/Submit.vue';

export default{
    name:'Form',
    components:{
        InputText,
        Submit
    },
    data(){
        return{
name:"",
email:""
        }
    },
    methods:{
        enviarFormulario(e){

e.preventDefault();
const name=this.name;
const email=this.email;

            console.log("Formulário Enviado.");
            console.log("o nome é:" + name);
            console.log("o nome é:" + email);
        }
    }
}
</script>
<style scoped>
p{
    margin: 50px;
}</style>