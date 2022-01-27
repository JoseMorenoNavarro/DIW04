<template>
  <section id="producto-imagen">
      <div class="img-big"> 
          <img v-bind:src="fotos[0]" alt="Portátil Lenovo 920" copyright="cc-0">
      </div>
        <div class="img-mini">
            <a @click="cambiarFoto(0)"><img  v-bind:src="fotos[0]" alt="Portátil Lenovo 920" copyright="cc-0"></a>
            <a @click="cambiarFoto(1)"><img  v-bind:src="fotos[1]" alt="Portátil Lenovo 920" copyright="cc-0"></a>
            <a @click="cambiarFoto(2)"><img  v-bind:src="fotos[2]" alt="Portátil Lenovo 920" copyright="cc-0"></a>
        </div>
      </section>    
</template>

<script>
export default {
    Name: 'ProductoImagen',
    data () {
        return {
            fotos: [
                require ('../assets/lap1.jpg'),
                require ('../assets/lap2.jpg'),
                require ('../assets/lap3.jpg')]
        }
    },
    methods: {
        cambiarFoto(id) {
            this.fotos[0] = this.fotos[id]
        }
    }
}
</script>

<style escoped>
#producto-imagen {
    border-radius: 25px;
    padding: 1rem;
    margin: 1rem;
    flex: 0 1 50%;
}
.img-mini {
    display: flex;
    justify-content: flex-start;
}
.img-mini img {
    width: 100px;
    border:2px solid #d8d8d8;
    
}
</style>