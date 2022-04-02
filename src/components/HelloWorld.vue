<template>
  <div class="hello">
    <h1>Pastelería Delicious!</h1>
    <p>Somos una pastelería mexicana especializada en materializar tus ideas y ofrecerte la mejor calidad del mercado.</p>
    <router-link to="/pedidos"><botonMorado texto="Inicia tu Pedido" /></router-link>
  </div>
</template>

<script>
import botonMorado from './botonMorado.vue'

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  components: {
    botonMorado,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello{
  text-align: left;
  width: 50%;
}
.hello p{
  font-family:Cambria, Cochin, Georgia, Times, 'Times New Roman', serif ;
}
</style>
