<template>
    <div>
        <h2>Esta é a descrição da pessoa: {{ nome }}</h2>
        <Info :email="email" :esta_trabalhando="true" /><!--Esse é o componente filho de Pessoa-->
        <From />
    </div>
</template>

<script>
    export default{
        name:'Pessoa',

        data(){
            return{
                nome: 'Augusto',
                email: 'augusto@email.com'
            }
        }
    }
</script>
