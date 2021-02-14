<template>
  <div id="app"> 
      <Headermaturite/>
      <DownHeader/>
      <Sobre/>
      <Planos/>
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


export default {
  name: 'App',
  components: {
    Headermaturite,
    DownHeader,
    Sobre,
    FooterMatutite,
    Contato,
    Planos
  }
}
</script>

 
<style>
  @-webkit-keyframes fadein{
  from { opacity: 0; transform: translateY(-500px); }
  to { opacity: 1; transform: translateY(0px);}
}

@-moz-keyframes fadein{
  from { opacity: 0; transform: translateY(-500px); }
  to { opacity: 1; transform: translateY(0px);}
}

@-o-keyframes fadein{
  from { opacity: 0; transform: translateY(-500px); }
  to { opacity: 1; transform: translateY(0px);}
}

@-ms-keyframes fadein{
  from { opacity: 0; transform: translateY(-500px); }
  to { opacity: 1; transform: translateY(0px);}
}

@keyframes fadein{
  from { opacity: 0; transform: translateY(-500px); }
  to { opacity: 1; transform: translateY(0px);}
}


  #app{
    -ms-animation: fadein 2.2s ease-in-out;
    -o-animation: fadein 2.2s ease-in-out;
    -moz-animation: fadein 2.2s ease-in-out;
    -webkit-animation: fadein 2.2s ease-in-out;
    animation: fadein 2.2s ease-in-out;
  }

</style>
