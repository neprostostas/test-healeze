<template>
  <MainLayout>
    <Main/>
  </MainLayout>
</template>

<script>
import MainLayout from './components/MainLayout.vue'
import Main from './components/Main.vue'

export default {
  name: 'App',
  components: {
    MainLayout,
    Main
  }
}
</script>

<style>

body, h1, h2, h3, h4, h5, p {
  margin: 0;
}

button {
  cursor: pointer;
}

* {
  /* transition: .5s all ease-in-out; */
}

</style>
