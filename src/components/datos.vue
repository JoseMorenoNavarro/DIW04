<template>
  <section id="producto-datos">
      <h1>PLenovo 920 13"</h1>
      <h2>750,69€ <span class="iva">sin IVA: 620,41€</span></h2>
      <div class="wrapper">
          <button class="btn" @click="cambiarContador('-1')" type="button" name="button">-</button>
          <input class="cantidad" type="text" name="name" :value="contador">
          <button class="btn" @click="cambiarContador('1')" type="button" name="button">+</button>
      </div>
      <br>
      <button class="boton">AÑADIR CARRITO</button>
  </section>
</template>

<script>
export default {
  Name: 'ProductoDatos',
    data () {
        return {
            contador: 1
        }
    },
    methods: {
        cambiarContador(num) {
            this.contador += +num;
            if (!isNaN(this.contador) && (this.contador < 0)) {
              this.contador = 0
            }
        }
    }
}
</script>

<style scoped>
section#producto-datos {
    margin-left: 1rem;
    flex: 1 1 18rem;
}
h1 {
    font-size: 2.2rem;
}
h2 {
    font-size:1.7rem;
    color: #0090ED;
}
span.iva {
    font-size:1rem;
    font-weight: normal;
    color: #282828
}
.wrapper {
    height: 2rem;
    display: flex;
}
.cantidad {
    border: none;
    text-align: center;
    width: 2rem;
    font-size: 1.2rem;
    border: 1px solid #d8d8d8;
}
.btn {
    border: 1px solid #d8d8d8;
    width: 1.8rem;
}
button:focus, input:focus {
    outline: 0;
}
.boton{
    text-decoration: none;
    padding: 10px;
    font-weight: 600;
    font-size: 20px;
    color: #ffffff;
    background-color: #1883ba;
    border-radius: 6px;
    border: 0px;
}
.boton:hover{
    text-decoration: none;
    padding: 10px;
    font-weight: 600;
    font-size: 20px;
    color: #ffffff;
    background-color: #ED5C00;
    border-radius: 6px;
    border: 0px;
}
</style>