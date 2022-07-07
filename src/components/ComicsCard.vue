<template>
  <div class="comics-card">
        <img :src="productDetails.thumb" :alt="productDetails.series">
        <h3>{{ productDetails.series }}</h3>
    </div>
</template>

<script>
export default {
    name: "ComicsCard",
    props: {
        productDetails : Object
    }

}
</script>

<style lang="scss" scoped>
@import '../style/variables';

.comics-card {
    width: calc((100% / 6) - 10px);
    margin: 5px;

    h3 {
        color: white;
        font-size: 1rem;
        font-weight: 300;
        margin: 0.5rem 0;
    }
}

</style>