<template>
  <div id="home">
    <div class="cont-nome">
      <h1>Alessandro Rega</h1>
    </div>
    <div class="sfondo">
      <img src="../assets/img/sfondo.png" alt="sfondo">
    </div>
    <div class="desktop">
      <div class="icone-programmi">
        <i class="fab fa-html5"></i>
        <i class="fab fa-js"></i>
        <i class="fab fa-laravel"></i>
        <i class="fab fa-css3-alt"></i>
        <i class="fab fa-sass"></i>
        <i class="fab fa-bootstrap"></i>
        <i class="fab fa-vuejs"></i>
        <i class="fab fa-php"></i>
      </div>
      <div class="quadrati">
        <img src="../assets/img/sfondo-desktop.png" alt="sfondo-desktop">
      </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'Home',
}
</script>

<style lang="scss" scoped>
// Importazione variabili
@import "../assets/style/variables.scss";

.cont-nome{
  width: 100%;
  height: 100vh;
  position: absolute;
  top: 0;
  left: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;

  h1{
    text-transform: uppercase;
    font-family: $Oswald;
    font-weight: 600;
    font-size: 60px;
    z-index: 1;
  }
}

.sfondo{
  width: 100%;
  height: 100vh;
  transform: translate(0, -17%);

  img{
    width: 150%;
    height: 115%;
    opacity: 0.85;
    transform: translate(-17%, -5%);
  }
}

.desktop{
  display: none;
}

@media screen and (min-width: 768px){
  .cont-nome{

    h1{
      width: 70%;
      font-size: 96px;
    }
  }
}
@media screen and (min-width: 1024px){
  .cont-nome{

    h1{
      width: 100%;
      font-size: 96px;
    }
  }

  .sfondo{

    img{
      filter: opacity(1);
    }
  }
}
@media screen and (min-width: 1440px){
  .sfondo{
    display: none;
  }

  .desktop{
    display: block;
    position: relative;
    width: 100%;
    height: calc(100vh - 200px);
  }

  .cont-nome{
    z-index: 3;
  }

  .quadrati{
    width: 100%;
    height: calc(100vh - 200px);
    z-index: -1;

    img{
      width: 150%;
      transform: translate(-18%, -35%);
    }
  }

  .icone-programmi{
    position: relative;
    z-index: 2;

    .fa-html5{
      font-size: 55px;
      position: absolute;
      top: 252px;
      left: 83px;
      transform: rotate(-9.58deg);
    }
    .fa-js{
      font-size: 55px;
      position: absolute;
      top: 132px;
      left: 458px;
      transform: rotate(-8.88deg);
    }
    .fa-laravel{
      font-size: 55px;
      position: absolute;
      top: 86px;
      left: 900px;
      transform: rotate(10.28deg);
    }
    .fa-css3-alt{
      font-size: 55px;
      position: absolute;
      top: 252px;
      left: 1293px;
      transform: rotate(6.98deg);
    }
    .fa-sass{
      font-size: 55px;
      position: absolute;
      top: 555px;
      left: 1136px;
    }
    .fa-bootstrap{
      font-size: 55px;
      position: absolute;
      top: 708px;
      left: 818px;
    }
    .fa-vuejs{
      font-size: 55px;
      position: absolute;
      top: 504px;
      left: 580px;
      transform: rotate(-6.47deg);
    }
    .fa-php{
      font-size: 55px;
      position: absolute;
      top: 517px;
      left: 235px;
      transform: rotate(3.63deg);
    }
  }
}
@media screen and (min-width: 1920px){
  .quadrati{

    img{
      width: 120%;
      transform: translate(-10%, -35%);
    }
  }

  .icone-programmi{
    position: relative;
    z-index: 2;

    .fa-html5{
      font-size: 80px;
      position: absolute;
      top: 280px;
      left: 246px;
      transform: rotate(-9.58deg);
    }
    .fa-js{
      font-size: 80px;
      position: absolute;
      top: 42px;
      left: 679px;
      transform: rotate(-8.88deg);
    }
    .fa-laravel{
      font-size: 80px;
      position: absolute;
      top: 89px;
      left: 1189px;
      transform: rotate(10.28deg);
    }
    .fa-css3-alt{
      font-size: 80px;
      position: absolute;
      top: 164px;
      left: 1619px;
      transform: rotate(6.98deg);
    }
    .fa-sass{
      font-size: 80px;
      position: absolute;
      top: 530px;
      left: 1460px;
    }
    .fa-bootstrap{
      font-size: 80px;
      position: absolute;
      top: 506px;
      left: 1094px;
    }
    .fa-vuejs{
      font-size: 80px;
      position: absolute;
      top: 371px;
      left: 819px;
      transform: rotate(-6.47deg);
    }
    .fa-php{
      font-size: 80px;
      position: absolute;
      top: 521px;
      left: 421px;
      transform: rotate(3.63deg);
    }
  }
}
</style>