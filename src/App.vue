<template>
  <div id="app"> 
        <img src="./assets/logo.svg" alt="Logo loading" id="initial-logo">
      <div id="page" >
        <Headermaturite/>
        <DownHeader/>
        <Sobre/>
        <Posts-depoimentos/>
        <Planos/>
        <Caracteristicas/>
        <Contato/>
        <Footer-matutite/>
      </div>
  </div>
</template>

<script>
import Headermaturite from './components/Header-maturite.vue'
import DownHeader from './components/Down-header.vue'
import Sobre from './components/Sobre'
import FooterMatutite from './components/Footer-matutite.vue'
import Contato from './components/Contato.vue'
import Planos from './components/Planos.vue'
import Caracteristicas from './components/Caracteristicas.vue'
import PostsDepoimentos from './components/Posts-depoimentos.vue'


export default {
  name: 'App',
  components: {
    Headermaturite,
    DownHeader,
    Sobre,
    FooterMatutite,
    Contato,
    Planos,
    Caracteristicas,
    PostsDepoimentos
  },
  mounted () {
    document.getElementById('page').className = 'animationIn'
  }
}
</script>

 
<style>
  @-webkit-keyframes fadeIn{
  from { opacity: 0; }
  to { opacity: 1; }
}

@-moz-keyframes fadeIn{
  from { opacity: 0; }
  to { opacity: 1; }
}

@-o-keyframes fadeIn{
  from { opacity: 0; }
  to { opacity: 1; }
}

@-ms-keyframes fadeIn{
  from { opacity: 0; }
  to { opacity: 1; }
}

@keyframes fadeIn{
  from { opacity: 0; }
  to { opacity: 1; }
}

@-webkit-keyframes fadeOut{
  from { opacity: 1; }
  to { opacity: 0;}
}

@-moz-keyframes fadeOut{
  from { opacity: 1; }
  to { opacity: 0;}
}

@-o-keyframes fadeOut{
  from { opacity: 1; }
  to { opacity: 0;}
}

@-ms-keyframes fadeOut{
  from { opacity: 1; }
  to { opacity: 0;}
}

@keyframes fadeOut{
  from { opacity: 1; }
  to { opacity: 0; }
}

.animationIn{
    -ms-animation: fadeIn 5.2s ease-in-out;
    -o-animation: fadeIn 5.2s ease-in-out;
    -moz-animation: fadeIn 5.2s ease-in-out;
    -webkit-animation: fadeIn 5.2s ease-in-out;
    animation: fadeIn 5.2s ease-in-out;
}

/*div .initial-logo{
  height: 100vh;
  width: 100vw;
  position: absolute;
  width: 25vw;
  height: 25vw;
  align-items: center;
  justify-content: center;
}*/

#initial-logo{
    position: fixed;
    height: 25vw;
    width: 25vw;
    
    left: 50%;
    margin-left: -12.5vw;
    
    top: 50%;
    margin-top: -12.5vw;

    -ms-animation: fadeOut 5.2s ease-in-out;
    -o-animation: fadeOut 5.2s ease-in-out;
    -moz-animation: fadeOut 5.2s ease-in-out;
    -webkit-animation: fadeOut 5.2s ease-in-out;
    animation: fadeOut 5.2s ease-in-out;

    opacity: 0;
}

</style>
