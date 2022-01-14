<template>
  <div id="home">
      <div class="cont-quadrati">
          <div class="quadrato-blu-destro"></div>
          <div class="quadrato-blu-sinistro"></div>
          <div class="quadrato-blu-centrale"></div>
          <div class="quadrato-blu-esterno-sinistro"></div>
          <div class="quadrato-blu-esterno-destro"></div>
          <div class="quadrato-rosso-destro"></div>
          <div class="quadrato-rosso-sinistro"></div>
          <div class="quadrato-rosso-centrale"></div>
          <div class="quadrato-rosso-esterno-sinistro"></div>
          <div class="quadrato-rosso-esterno-destro"></div>
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

#home{
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;

    .cont-quadrati{
        width: 375px;
        height: 667px;
        position: relative;

        .quadrato-blu-destro{
            position: absolute;
            width: 200px;
            height: 200px;
            right: -100px;
            top: 60px;
            border: 10px solid $quadrato-blu-sfocato;
            transform: matrix(0.71, 0.7, 0.7, -0.71, 0, 0);
            z-index: -1;
        }
        .quadrato-blu-sinistro{
            position: absolute;
            width: 200px;
            height: 200px;
            left: -100px;
            top: 70px;
            border: 10px solid $quadrato-blu-sfocato;
            transform: rotate(37.67deg);
            z-index: -1;
        }
        .quadrato-blu-centrale{
            position: absolute;
            width: 200px;
            height: 200px;
            left: 60px;
            bottom: -40px;
            border: 10px solid $quadrato-blu-sfocato;
            transform: rotate(-79.63deg);
            z-index: -1;
        }
        .quadrato-blu-esterno-sinistro{
            position: absolute;
            width: 200px;
            height: 200px;
            left: -230px;
            bottom: 10px;
            border: 10px solid $quadrato-blu-sfocato;
            transform: matrix(0.28, 0.96, 0.96, -0.28, 0, 0);
            z-index: -1;
        }
        .quadrato-blu-esterno-destro{
            position: absolute;
            width: 200px;
            height: 200px;
            right: -230px;
            bottom: 10px;
            border: 10px solid $quadrato-blu-sfocato;
            transform: matrix(0.28, 0.96, 0.96, -0.28, 0, 0);
            z-index: -1;
        }
        .quadrato-rosso-destro{
            position: absolute;
            width: 200px;
            height: 200px;
            right: -75px;
            bottom: 70px;
            border: 10px solid $quadrato-rosso-sfocato;
            transform: rotate(-109.63deg);
            z-index: -1;
        }
        .quadrato-rosso-sinistro{
            position: absolute;
            width: 200px;
            height: 200px;
            left: -100px;
            bottom: 100px;
            border: 10px solid $quadrato-rosso-sfocato;
            transform: rotate(-46.07deg);
            z-index: -1;
        }
        .quadrato-rosso-centrale{
            position: absolute;
            width: 200px;
            height: 200px;
            left: 80px;
            top: -50px;
            border: 10px solid $quadrato-rosso-sfocato;
            transform: matrix(0.28, 0.96, 0.96, -0.28, 0, 0);
            z-index: -1;
        }
        .quadrato-rosso-esterno-sinistro{
            position: absolute;
            width: 200px;
            height: 200px;
            left: -280px;
            top: -10px;
            border: 10px solid $quadrato-rosso-sfocato;
            transform: matrix(0.28, 0.96, 0.96, -0.28, 0, 0);
            z-index: -1;
        }
        .quadrato-rosso-esterno-destro{
            position: absolute;
            width: 200px;
            height: 200px;
            right: -280px;
            top: -10px;
            border: 10px solid $quadrato-rosso-sfocato;
            transform: matrix(0.28, 0.96, 0.96, -0.28, 0, 0);
            z-index: -1;
        }
    }
}

@media screen and (min-width: 768px){}
@media screen and (min-width: 1024px){}
@media screen and (min-width: 1440px){}
@media screen and (min-width: 1920px){}
</style>