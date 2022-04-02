<template>
  <div class="home">
    <HelloWorld class="textoHome" msg="Holiwi uwu"/>
    <img alt="Vue logo" src="../assets/img/Group7.png">
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld,
  },
  watch:{
    $route: {
      immediate: true,
      handler(to) {
        document.title = to.meta.title || 'Delicious! - Home'
      }
    }
  }
}
</script>

<style>
.home {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
}

.home img{
  width: 40vw;
  padding-left: 2vw;
}

.home .textoHome{
  width: 33vw;
  text-align: left;
  font-size: 1.2vw;
}
</style>