<template>
    <div class="product-card">
        <img :src="immagine" alt="titolo">
        <h3>{{titolo}}</h3>
    </div>
</template>
<script>
export default {
    nome:'ProductCard',
    data(){
        return{

        }

    },
    props:['immagine','titolo']
}
</script>
<style lang="scss" scoped>
@import '../style/variables';

    .product-card{
        width: calc(100% / 4 - 10px);
        background-color: white;
        padding: 5px;
        margin: 5px;
        img{
            max-width: 100%;
        }
        h3{
            text-align: center;
            font-size: 1em;
            color: $primaryText;
        }
    }
</style>