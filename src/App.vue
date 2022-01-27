<template>
  <Cabecera />
  <Menu />
  <Migas />
  <Imagenes />
  <Datos />
  <Descripcion />
  <Footer />
</template>

<script>
import Cabecera from './components/cabecera.vue'
import Menu from './components/menu.vue'
import Migas from './components/migas.vue'
import Imagenes from './components/imagenes.vue'
import Datos from './components/datos.vue'
import Footer from './components/footer.vue'
import Descripcion from './components/descripcion.vue'


export default {
  name: 'App',
  components: {
    Cabecera, Menu, Migas, Footer, Descripcion, Imagenes, Datos
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@500&display=swap');
body{
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
}
.container {
    max-width: 1400px;
    margin: auto;
}
#app {
  font-family: 'Open Sans', sans-serif;
}
</style>
