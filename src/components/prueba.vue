<template>
<h2>{{funcion}}</h2>
</template>

<script>
export default{
    name: 'conter',
    data(){
        return{
            conter: 5
        }
    },
    computed: {
        funcion(){
            return this.conter * this.conter
        }
    }
}
</script>