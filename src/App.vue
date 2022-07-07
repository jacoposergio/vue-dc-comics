<template>
  <div id="app">
    <PageHeader/>
    <PageComics/>
    <PageMain/>
    <PageFooter/>
  </div>
</template>

<script>
 import PageHeader from './components/PageHeader.vue';
 import PageMain from './components/PageMain.vue';
 import PageComics from './components/PageComics.vue'; 
 import PageFooter from './components/PageFooter.vue';

export default {
    name: 'App',
    components: {
      PageHeader,
      PageMain,
      PageComics,
      PageFooter,
  },
};
</script>

<style lang="scss">
@import './style/common.scss';
@import './style/variables.scss';
</style>
