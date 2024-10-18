<template>
    <div>
        <Reutilizacao />
        <h1>Olá Vue!</h1>
        <p>Meu nome é {{ nome }} e trabalho como {{ profissao }}</p>
        <MultiplosEventos />
        
    </div>
</template>

<script>
import Reutilizacao from './Reutilizacao.vue';
import MultiplosEventos from './MultiplosEventos.vue';

 export default {
    name: 'PrimeiroComponente',
    components: {
        Reutilizacao,
        MultiplosEventos
    },
    data(){
        return {
            nome: "Augusto",
            profissao: "Programador"
        }
    }
 }
</script>