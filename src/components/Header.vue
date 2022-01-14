<template>
  <header>
      <h2>Full Stack Web Developer</h2>
      <div class="burger-menu">
          <i class="fas fa-bars" v-on:click="menu_open"></i>
      </div>
      <div class="classic-menu">
          <ul>
              <li><a href="#">Home</a></li>
              <li><a href="#">About</a></li>
              <li><a href="#">Works</a></li>
          </ul>
      </div>

      <!-- Menu a comparsa -->
      <div class="burger-menu-open" :class="open ? 'open' : 'closed'">
          <i class="fas fa-times" v-on:click="menu_closed"></i>
          <ul>
              <li v-on:click="menu_closed"><a href="#">Home</a></li>
              <li v-on:click="menu_closed"><a href="#">About</a></li>
              <li v-on:click="menu_closed"><a href="#">Works</a></li>
          </ul>
      </div>
  </header>
</template>

<script>
export default {
    name: 'Header',
    data(){
        return{
            open: false
        }
    },
    methods:{
        menu_open: function (){
            this.open = true;
        },
        menu_closed: function(){
            this.open = false;
        }
    }
}
</script>

<style lang="scss" scoped>
// Importazione variabili
@import "../assets/style/variables.scss";

// Media-Query 375px
header{
    // Dimensioni
    width: 100%;
    height: 100px;
    // Display
    display: flex;
    justify-content: space-between;
    align-items: center;
    //------//
    position: relative;

    h2{
        font-family: $Lobster;
        font-weight: normal;
        font-size: 20px;
        margin-left: 17px;
    }

    .burger-menu{
        text-align: center;
        margin-right: 27px;
        cursor: pointer;

        i{
            font-size: 30px;
        }
    }

    .classic-menu{
        display: none;
    }

    .burger-menu-open{
        width: 100%;
        height: 100vh;
        position: absolute;
        top: 0;
        left: 0;
        background-color: #fff;

        &::after{
            content: "";
            clear: both;
            display: table;
        }

        i{
            font-size: 30px;
            float: right;
            margin-right: 27px;
            margin-top: 25px;
            cursor: pointer;
        }

        ul{
            width: 143px;
            height: 400px;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            align-items: center;
            list-style: none;

            li{
                font-size: 30px;
                font-family: $Lato;

                a{
                    text-decoration: none;
                    color: black;
                }
            }
        }
    }

    .closed{
        left: +100%;
        transition: 0.5s ease-in-out;
    }

    .open{
        left: 0%;
        transition: 0.5s ease-in-out;
    }
}

// Tablet Mini
@media screen and (min-width: 768px){
    header{
        height: 200px;

        h2{
            font-size: 36px;
            margin-left: 21px;
        }

        .burger-menu{
            i{
                font-size: 50px;
            }
        }

        .burger-menu-open{
            ul{
                height: 600px;

                li{
                    font-size: 50px;
                }
            }

            i{
                font-size: 50px;
            }
        }
    }

}

// Tablet
@media screen and (min-width: 1024px){
}

// Portatile
@media screen and (min-width: 1440px){
    header{

        h2{
            margin-left: 51px;
        }

        .burger-menu{
            display: none;
        }

        .classic-menu{
            width: 370px;
            height: 30px;
            display: block;
            margin-right: 86px;

            ul{
                list-style: none;
                display: flex;
                justify-content: space-between;
                align-items: center;

                li{
                    font-family: $Lato;
                    font-size: 18px;

                    &:hover{
                        text-decoration: underline;
                    }

                    a{
                        text-decoration: none;
                        color: black;
                    }
                }
            }
        }

        .burger-menu-open{
            display: none;
        }
    }
}

// Desktop
@media screen and (min-width: 1920px){
    header{

        h2{
            margin-left: 167px;
        }
    }
}
</style>