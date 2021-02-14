<template>
  <div id="app"> 
      <Headermaturite/>
      <DownHeader/>
      <Sobre/>
      <Planos/>
      <Caracteristicas/>
      <Contato/>
      <Footer-matutite/>
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


export default {
  name: 'App',
  components: {
    Headermaturite,
    DownHeader,
    Sobre,
    FooterMatutite,
    Contato,
    Planos,
    Caracteristicas
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

#app{
    -ms-animation: fadeIn 2.2s ease-in-out;
    -o-animation: fadeIn 2.2s ease-in-out;
    -moz-animation: fadeIn 2.2s ease-in-out;
    -webkit-animation: fadeIn 2.2s ease-in-out;
    animation: fadeIn 2.2s ease-in-out;
}

</style>
