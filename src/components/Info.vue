<template>
    <div>
<p v-if="esta_trabalhando">Estou trabalhando no momento</p>
<p v-else="esta_trabalhando">Estou em busca de novas oportunidades</p>
<p>Utilizo as seguintes tecnologias para backend:</p>
<ul >
  <li v-for="(technology, index) in backend_technologies" v-bind:key="index">{{ technology }}</li>
</ul>
<p>Utilizo as seguintes tecnoloias para front-end:</p>
<ul>
 <li v-for="technology in frontend_tecnologies":key="technology.id">{{ technology.language }}</li> 
</ul>
<button @click="showEmail">{{ textoBotao }}</button>
<p v-show="mostrar_email">Mande uma mensagem para:{{ email }}</p>
<p class="teste">Para acessar meu Portifólio <a v-bind:href="meu_link"target="_blank"> Basta clicar aqui.</a></p>
<Picture></Picture>
</div>
</template>

<script>


import Picture from './Picture.vue';
export default{
    name:'Info',
    components:{
        Picture
    },
    data(){
        return{
            esta_trabalhando:true,
            mostrar_email:true,
            email:'adycbranco@gmail.com',
            meu_link:'http://www.staggeringbeauty.com/',
            textoBotao:'Mostrar e-mail',
            backend_technologies:['javaScript', 'PHP', 'Phyton'],
            frontend_tecnologies:[
                {id:1,language:'HTML'},
                 {id:2,language:'CSS'},
                  {id:3,language:'Vue'},
            ]
        }
    },
    methods:{
        showEmail(){
            this.mostrar_email=!this.mostrar_email
            if(this.mostrar_email){
this.textoBotao='Mostrar E-mail'
            }else{
                this.textoBotao='Esconde e-mail'
            }
        }

    }
}
</script>
https://google.com