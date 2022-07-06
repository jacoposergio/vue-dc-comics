<template>
  <div id="app">
    <PageHeader/>
    <PageMain/>
  </div>
</template>

<script>
 import PageHeader from './components/PageHeader.vue';
 import PageMain from './components/PageMain.vue';

export default {
    name: 'App',
    components: {
      PageHeader,
      PageMain,
  },
};
</script>

<style lang="scss">
@import './style/common.scss';
@import './style/variables.scss';
</style>
