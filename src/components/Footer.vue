<template>
  <div class="CustomFooter">
    <footer>
      {{txt}}
    </footer>
  </div>
</template>

<script>

export default {
  name: 'CustomFooter',
  props: {
    txt: String
  }
}
</script>

<style scoped>

  .CustomFooter {
    padding: 25px 71px;
    font-family: 'Helvetica Neue';
    font-style: normal;
    font-weight: 400;
    font-size: 14px;
    line-height: 12px;
    color: #000000;
  }

</style>
