<template>
  <div class="textLine">

    <div class="textWrapper">
       <p>{{txt}}</p>
    </div>

    <div class="arrowWrapper">
        <svg class="arrow" width="20" height="19" viewBox="0 0 20 19" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M4.70236 0.253021L4.8971 3.70117L12.613 4.09721L0.938472 15.7718L3.49211 18.3254L15.1667 6.65085L15.5627 14.3668L19.0109 14.5615L18.3123 0.951461L4.70236 0.253021Z" fill="#20B472"/>
        </svg>
    </div>

  </div>
</template>

<script>

export default {

  name: 'textLine',
  props: {
    txt: String
  }

}
</script>

<style scoped>

    .textLine {
        display: grid;
        grid-template-columns: repeat(2, auto);
        align-items: center;
        justify-content: start;
        gap: 20px;
        width: fit-content;
    }

    .arrowWrapper {
        display: grid;
        width: 86px;
        height: 86px;
        border: 1px solid #E6E6E6;
        border-radius: 50%;
    }

    .textLine:hover svg path {
        transition: .5s all ease-in-out;
        fill: #FFFFFF;
    }

    .textLine:hover .arrowWrapper {
        transition: .5s all ease-in-out;
        background: #29ABE2;
    }

    .textWrapper svg {
        align-self: center;
        margin: 0 auto;
    }

</style>
