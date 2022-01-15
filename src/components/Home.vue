<template>
  <div id="home-bassa">
    <div class="cont-nome">
      <h1>Alessandro Rega</h1>
    </div>
    <div class="icone">
      <div>
      <i class="fab fa-html5"></i>
      <i class="fab fa-js"></i>
      <i class="fab fa-laravel"></i>
      <i class="fab fa-css3-alt"></i>
      <i class="fab fa-sass"></i>
      <i class="fab fa-bootstrap"></i>
      <i class="fab fa-vuejs"></i>
      <i class="fab fa-php"></i>
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

#home-bassa{
  width: 100%;
  height: calc(100vh - 100px);
  display: flex;
  justify-content: center;
  align-items: center;
  background-image: url("../assets/img/sfondo.png");
  background-size: 800px;
  background-position: center;
  background-attachment: fixed;
}

.cont-nome{
  text-align: center;

  h1{
    text-transform: uppercase;
    font-family: $Oswald;
    font-weight: 600;
    font-size: 60px;
  }
}

.icone{
  display: none;
}

@media screen and (min-width: 768px){
  #home-bassa{
    height: calc(100vh - 200px);
  }

  .cont-nome{

    h1{
      font-size: 96px;
    }
  }
}
@media screen and (min-width: 1024px){
  .cont-nome{

    h1{
      font-size: 96px;
    }
  }
}
@media screen and (min-width: 1440px){
  #home-bassa{
    background-image: url("../assets/img/sfondo-desktop.png");
    background-size: 1600px;
    background-position: center;
  }

  .icone{
    display: block;
    width: 100%;
    height: 100vh;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);

    div{
      position: relative;
      width: 1400px;
      height: 800px;
      margin: 0 auto;
      top: 50%;
      transform: translateY(-50%);
    }
  }

  .fa-html5{
  font-size: 55px;
  position: absolute;
  top: 310px;
  left: 83px;
  transform: rotate(-9.58deg);
  }
  .fa-js{
    font-size: 55px;
    position: absolute;
    top: 180px;
    left: 458px;
    transform: rotate(-8.88deg);
  }
  .fa-laravel{
    font-size: 55px;
    position: absolute;
    top: 280px;
    left: 900px;
    transform: rotate(10.28deg);
  }
  .fa-css3-alt{
    font-size: 55px;
    position: absolute;
    top: 380px;
    right: 100px;
    transform: rotate(6.98deg);
  }
  .fa-sass{
    font-size: 55px;
    position: absolute;
    top: 630px;
    right: 250px;
  }
  .fa-bootstrap{
    font-size: 55px;
    position: absolute;
    top: 708px;
    right: 550px;
  }
  .fa-vuejs{
    font-size: 55px;
    position: absolute;
    top: 620px;
    left: 520px;
    transform: rotate(-6.47deg);
  }
  .fa-php{
    font-size: 55px;
    position: absolute;
    top: 550px;
    left: 210px;
    transform: rotate(3.63deg);
  }
}
@media screen and (min-width: 1920px){
  #home-bassa{
    background-size: 2070px;
  }
  .cont-nome{
    h1{
      font-size: 120px;
    }
  }

  .icone{

    div{
      width: 1900px;
    }
  }

  .fa-html5{
    font-size: 80px;
    top: 300px;
    left: 246px;
  }
  .fa-js{
    font-size: 80px;
    top: 180px;
    left: 679px;
  }
  .fa-laravel{
    font-size: 80px;
    top: 250px;
    left: 1189px;
  }
  .fa-css3-alt{
    font-size: 80px;
    top: 370px;
    right: 200px;
  }
  .fa-sass{
    font-size: 80px;
    top: 640px;
    right: 370px;
  }
  .fa-bootstrap{
    font-size: 80px;
    top: 670px;
    right: 780px;
  }
  .fa-vuejs{
    font-size: 80px;
    top: 580px;
    left: 700px;
  }
  .fa-php{
    font-size: 80px;
    top: 600px;
    left: 380px;
  }
}
</style>