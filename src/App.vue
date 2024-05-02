<script>
// import HelloWorld from './components/HelloWorld.vue'
import MyHeader from './components/MyHeader.vue';
import MyMain from './components/MyMain.vue';
import MyIcons from './components/MyIcons.vue';
import MyFooter from './components/MyFooter.vue';

export default {
  components: {
    MyHeader,
    MyMain,
    MyIcons,
    MyFooter,
  }
}
</script>

<template>

  <MyHeader />
  <MyMain />
  <MyIcons /> 
  <MyFooter />
</template>

<style lang="scss">


</style>
