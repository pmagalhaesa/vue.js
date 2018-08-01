<template>
    <div class="card" v-bind:class="['card--'+cor]">
        <p class="card__title">{{ titulo }}</p>
        <p class="card__description">{{ descricao }}</p>
    </div>
</template>

<script>
export default {
    name: 'Card',
    props:{
        titulo: String,
        descricao: String,
        cor: String
    }
}
</script>

<style scoped>
    .card{
        background-color: #d234bc;
        display: inline-block;
        padding: 15px 50px;
        margin: 0 5px;
        width: 138px;
    }
   
    .card--azul{
        background-color: #00bdd7;
    }
    .card--verde{
        background-color: #6cc43c;
    }
    .card--roxo{
        background-color: #bb68e0;
    }

    .card p{
        color: #fff;
    }
    .card__title{
        font-size:20px;
        font-weight:700;
        margin:0;
    }
    .card__description{
        font-size:10px;
        text-transform: uppercase;
        margin:0;
    }
    
</style>