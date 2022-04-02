<template>
  <div class="pedidos">
    <h1>Pedidos</h1>
    <h4>Sabores:</h4>
  </div>
</template>

<script>
export default {
  name: 'PedidosView',
  watch:{
    $route: {
      immediate: true,
      handler(to) {
        document.title = to.meta.title || 'Delicious! - Pedidos'
      }
    }
  }
}
</script>

<style scoped>
.pedidos {
  display: flex;
  flex-direction: column;
  justify-content:center;
  text-align: left;
  width: 73%;
  margin: auto;
}

.pedidos h1 {
  font-size: 2.5vw;
  margin-bottom: 0;
}

.pedidos h4 {
  font-size: 1.5vw;
  margin-bottom: 0;
}
</style>