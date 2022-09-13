<template>
  <div class="MainLayout">
    <CustomHeader/>
    <main>
      <slot/>
    </main>
    <CustomFooter txt="©2022. Laboworq LLC company"/>
  </div>
</template>

<script>

import CustomHeader from '../components/Header.vue'
import CustomFooter from '../components/Footer.vue'

export default {
  name: 'MainLayout',
  components: {
    CustomHeader,
    CustomFooter,
  }

}
</script>


<style scoped>

</style>
