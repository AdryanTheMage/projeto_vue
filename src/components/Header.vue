<template>
    <div>
        <ul>
            <li><a href="#">Home</a></li>
               <li><a href="#">Projetos</a></li>
                  <li><a href="#">Contatos</a></li>
                 
        </ul>
    </div>
</template>
<script>
export default{
    name:'Header'
}
</script>
<style scoped>
ul{
    list-style:none;
    display: flex;
    background-color: grey;
}
li{
    margin-right: 20px;
}
a{
    color:#ddd;
    text-decoration: none;
    transition: 0.5s;
    
}
a:hover{
    color:deeppink;

}
</style>