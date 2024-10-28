<template>
    <h1>Meu nome é {{ nome }}</h1>
</template>

<script>
    export default {
        name: 'LyfeCycle',
        data() {
            return {
                nome: 'eu mesmo'
            }
        },
        created() {
            setTimeout(() => {
                this.nome = "João"
            }, 1000)
            setTimeout(() => {
                this.nome = "Pedro"
            }, 2000)
            this.nome = "Daniel"
        },
        mounted() {
            this.nome = "Carlos"
        }
    }
</script>