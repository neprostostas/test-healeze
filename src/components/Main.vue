<template>
  <div class="CustomMain">

    <div class="xlImageWrapper">
      <img src="../assets/lg-pic.png" alt="lg-pic">
    </div>

    <div class="mainImages">
      <img src="../assets/xs-pic-1.png" alt="xs-pic-1">
      <img src="../assets/xs-pic-2.png" alt="xs-pic-2">
    </div>

    <div class="textBlock">

      <h1 class="textFirst">What Do You Want to Do?</h1>

      <div class="textWrapper">
        <template v-for="(txt, id) in texts" :key=id>
          <Textline :txt="txt"/>
        </template>
      </div>

    </div>

  </div>
</template>

<script>
import Textline from '../components/Textline.vue'

export default {
  name: 'CustomMain',
  components: {
    Textline
  },
  setup() {
    const texts = ["Find A Test Station", "My Applications", "Additional Services", "FAQ"]

    return { texts }
  }
}
</script>

<style scoped>

  .xlImageWrapper {
    position: absolute;
    top: 15%;
    right: 0;
  }

  .CustomMain {
    padding: 74px 71px 0;
  }

  .mainImages {
    display: grid;
    grid-template-columns: repeat(2, auto);
    justify-content: start;
    align-items: center;
    justify-items: center;
    gap: 15px;
  }

  .mainImages img:hover {
    position: relative;
    top: 2px;
  }

  .textFirst {
    padding-top: 73px;
    text-transform: uppercase;
    font-family: 'Helvetica Neue';
    font-style: normal;
    font-weight: 400;
    font-size: 23.4313px;
    line-height: 26px;
    text-transform: uppercase;
    color: #000000;
  }

  .textWrapper {
    padding: 43px 0 20px;
  }

  .textWrapper div {
    font-family: 'Helvetica Neue';
    font-style: normal;
    font-weight: 300;
    font-size: 75px;
    line-height: 90px;
    color: #DDDDDD;
  }

  .textWrapper div:hover {
    cursor: pointer;
    color: #29ABE2;
    transition: .5s all ease-in-out;
  }

</style>
