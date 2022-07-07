<template>
  <div class="jumbo-cards-container">
    <div class="jumbotron">
        <div class="current-series">
            <h3>CURRENT SERIES</h3>
        </div>
        <div class="jumbo-img">
            <img src="../assets/img/jumbotron.jpg" alt="jumbotron">
        </div>
    </div>
    <div class="comics-list">
        <ComicsCard  v-for="element, index in products" :key="index" :productDetails="element" />
    </div>
    <div class="load-more">
        <a href="#">LOAD MORE</a>
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

  .jumbo-cards-container{
    background-color: black;

        .jumbotron{
            height: 300px;

            .current-series{
                position: relative;
                width: 70%;
                margin: 0 auto;
              

                h3{
                    position: absolute;
                    top: 280px;
                    left: -10px;
                    color: white;
                    background-color: $brand_main_color;
                    padding: 0.5rem 1rem;
                }
            }
    
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
    
        .load-more{
            text-align: center;   
    
            a{
                text-align: center;
                background-color: $brand_main_color;
                display: inline-block;
                color: white;
                padding: 0.3rem 2rem;
                margin-bottom: 1.5rem;
                font-size: 0.8rem;
                font-weight: 500;
            }
        }
  }
</style>