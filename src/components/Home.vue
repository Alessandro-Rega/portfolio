<template>
  <div id="home">
    <div class="cont-nome">
      <h1>Alessandro Rega</h1>
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
  width: 100%;
  height: calc(100vh - 100px);
  display: flex;
  justify-content: center;
  align-items: center;
  border: 1px solid red;
}

.cont-nome{
  text-align: center;
  border: 1px solid lime;

  h1{
    text-transform: uppercase;
    font-family: $Oswald;
    font-weight: 600;
    font-size: 60px;
    z-index: 1;
  }
}

@media screen and (min-width: 768px){
  #home{
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
@media screen and (min-width: 1440px){}
@media screen and (min-width: 1920px){
  .cont-nome{
    h1{
      font-size: 120px;
    }
  }
}
</style>