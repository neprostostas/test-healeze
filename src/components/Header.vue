<template>
  <div class="CustomHeader">
    <header>
      <div class="headerWrapper">

        <img class="logoHealeze" src="../assets/logoHealeze.png" alt="logoHealeze">

        <div class="userBlock">
          <img src="../assets/ava.png" alt="userAvatar">
          <p>Steve Austin</p>
        </div>

        <div class="buttonsBlock">

          <div class="socialMediaBlock">
            <div class="playMarketButton">
              <img src="../assets/play-market.svg" alt="play-market">
            </div>
            <div class="appleButton">
              <img src="../assets/apple.svg" alt="apple">
            </div>
          </div>

          <button class="testButton">Test Registration</button>
          <button class="testButtonMobile">Reg</button>

          <img src="../assets/burger.svg" alt="burger">

        </div>

      </div>
    </header>
  </div>
</template>

<script>

export default {
  name: 'CustomHeader',
}
</script>

<style scoped>

  .CustomHeader {
    position: fixed;
    padding: 35px 71px 16px;
    border-bottom: 0.5px solid grey;
    background: #FFFFFF;
    z-index: 99;
    left: 0;
    right: 0;
  }

  .headerWrapper {
    display: grid;
    grid-template-columns: repeat(3, 33.3333%);
    align-items: center;
  }

  .buttonsBlock {
    display: grid;
    grid-template-columns: repeat(3, auto);
    justify-items: center;
    align-items: center;
    justify-content: end;
    gap: 40px;
  }

  .userBlock {
    display: grid;
    gap: 5px;
  }

  .socialMediaBlock {
    display: grid;
    justify-content: center;
    align-items: center;
    justify-items: center;
    grid-template-columns: repeat(2, auto);
    gap: 9.5px;
  }

  .socialMediaBlock div {
    width: 45px;
    height: 45px;
    display: grid;
    border: 1px solid #E8E8E8;
    border-radius: 50%;
  }
  
  .socialMediaBlock div img {
    margin: 0 auto;
    align-self: center;
  }

  .logoHealeze {
    width: 226px;
    height: 71px;
    transition: .5s all ease-in-out;
  }

  .logoHealeze:hover {
    transform: scale(1.02);
    transition: .5s all ease-in-out;
  }

  .userBlock {
    display: grid;
    justify-content: center;
    align-items: center;
    justify-items: center;
  }

  .userBlock img {
    border-radius: 50%;
  }

  .userBlock p {
    font-family: 'Helvetica Neue';
    font-style: normal;
    font-weight: 400;
    font-size: 14px;
    line-height: 21px;
    text-align: center;
    color: #000000;
  }

  .testButtonMobile {
    display: none;
  }

  .testButton, .testButtonMobile {
    background: #20B472;
    border: 1px solid #20B472;
    border-radius: 28px;
    font-family: 'Helvetica Neue';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 17px;
    text-align: center;
    color: #FFFFFF;
    padding: 22px 25px;
  }

  .testButton:hover, .testButtonMobile:hover {
    background: #0c824d;
    border: 1px solid #0c824d;
  }

  @media screen and (max-width: 1288px) {

    .testButton {
      display: none;
    }

    .testButtonMobile {
      padding: 12px 15px;
      display: unset;
    }

  }

  @media screen and (max-width: 835px) {

    .buttonsBlock {
      gap: 20px;
    }

    .socialMediaBlock {
      display: none;
    }

    .buttonsBlock {
      grid-template-columns: repeat(2, auto);
    }

    .headerWrapper {
      display: grid;
      grid-template-columns: repeat(3, auto);
      align-items: center;
    }

    .logoHealeze {
      width: 100px;
      height: unset;
    }

  }

  @media screen and (max-width: 500px) {
      .CustomHeader {
      padding: 35px 20px 16px;
    }
  }


</style>