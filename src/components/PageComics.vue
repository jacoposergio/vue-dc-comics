<template>
  <div>
    <div class="jumbotron">
        <div class="jumbo-img">
            <img src="../assets/img/jumbotron.jpg" alt="jumbotron">
        </div>
    </div>
    <div class="comics-list">
        <ComicsCard  v-for="element, index in products" :key="index" :productDetails="element" />
    </div>
    <div class="load-more">

    </div>
  </div>
</template>

<script>
import productsJson from '../assets/dc-comics.json';
import ComicsCard from './ComicsCard.vue';

export default {
    name: 'PageComics',
    components: {
        ComicsCard
    },
     data() {
        return {
            products: productsJson
        };
    }
}
</script>

<style lang="scss" scoped>
  @import '../style/variables.scss';
    .jumbotron{
        height: 300px;

        .jumbo-img{
            height: 100%;
            overflow: hidden;
        }
    }

    .comics-list{
        margin: 2rem auto;
        width: 70%;
        display: flex;
        flex-wrap: wrap;
    }
</style>