<template>
    <div>
        <img :src="avatar" :alt="descricao">
        <MudarImagem @mudar-imagem="trocarImagem" />
    </div>
</template>

<script>
import MudarImagem from './MudarImagem.vue'

export default {
    name: 'Picturee',
    components: {
        MudarImagem
    },
    data(){
        return{
            avatar:"/img/avatar.png",
            descricao: "Augusto Liberato"
        }
    },
    methods: {
        trocarImagem(){
            this.avatar = "/img/avatar2.png"
        }
    }
}
</script>