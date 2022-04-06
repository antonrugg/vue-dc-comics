<template>
  <div id="app">
    <HeaderComponent/>
    <MainComponent/>
    <BlueSectionComponent/>
    <FooterComponent/>
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import MainComponent from './components/MainComponent.vue'
import BlueSectionComponent from './components/BlueSectionComponent.vue'
import FooterComponent from './components/FooterComponent.vue'

export default {
  name: 'App',
  components: {
      HeaderComponent,
      MainComponent,
      BlueSectionComponent,
      FooterComponent,
  }
}
</script>

<style lang="scss">

*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.container-90w{
  margin: auto 100px;
}

</style>
