<template>
    <div>
        <p>{{ compEmail }} - {{ email }}</p>
        <p v-if="esta_trabalhando"> Estou trabalhando no momento</p>
        <p v-else>Estou em busca de nova oportunidade</p>
        <p>Utilizo tecnologias para back-end:</p>

        <ul>
            <li v-for="(technology, index) in backend_technologies" v-bind:key="index">
                {{ technology }}
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
    name: 'Info',
    data(){
        return {
            backend_technologies: ['JavaScript', 'PHP', 'Python'],
            frontend_technologies: [
                {id: 1, language: 'HTML'},
                {id: 2, language: 'CSS'},
                {id: 3, language: 'Vue'}
            ]
        }
    }
}
</script>
