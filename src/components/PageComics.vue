<template>
  <div>
    <div class="jumbotron">
        <div class="jumbo-img">
            <img src="../assets/img/jumbotron.jpg" alt="jumbotron">
        </div>
    </div>
    <div class="comics-list">
        comic
    </div>
    <div class="load-more">

    </div>
  </div>
</template>

<script>
export default {
    name: 'PageComics',

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
</style>