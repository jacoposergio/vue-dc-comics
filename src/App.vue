<template>
  <div id="app">
    <PageHeader/>
    <PageComics/>
    <PageMain/>
  </div>
</template>

<script>
 import PageHeader from './components/PageHeader.vue';
 import PageMain from './components/PageMain.vue';
 import PageComics from './components/PageComics.vue'; 

export default {
    name: 'App',
    components: {
      PageHeader,
      PageMain,
      PageComics,
  },
};
</script>

<style lang="scss">
@import './style/common.scss';
@import './style/variables.scss';
</style>
