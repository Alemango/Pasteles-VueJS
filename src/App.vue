<template>
  <div>
    <nav>
      <router-link to="/"><img src="./assets/img/Logo.png" alt="logo"></router-link>
      <router-link to="/pedidos">Pedidos</router-link>
      <router-link to="/admin">Administración</router-link>
      <router-link to="/about">Contacto</router-link>
    </nav>
    <router-view/>
    <footer class="footer">
      <div class="container">
        <p>Av. Morelos 15 Col. Coaxusco, Tepetlixpa, Estado de México. Teléfono. 55 2011 9463. Atención. Lunes a Viernes 9.00 am a 16.00 pm, Sábados 9.00 am a 13.00 pm</p>
        <h4>Diseñado por <a target="_blank" href="https://linktr.ee/alemango">@Alemango</a></h4>
      </div>
    </footer>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Righteous&display=swap');

body{
  background-image: url("./assets/background.png");
  background-size: cover;
  background-repeat: no-repeat;
}

#app {
  font-family: 'Righteous', cursive;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #333;
}

nav {
  margin-left: 10vw;
  display: flex;
  align-items: center;
  font-size: 1.2vw;
}

nav a {
  color: #333;
  text-decoration: none;
  padding-left: 3vw;
}

nav a:hover{
  color: rgb(150, 41, 150);
  font-weight: bolder;
}

nav a.router-link-exact-active {
  color: rgb(150, 41, 150);
  font-weight: bold;
}

nav a img{
  width: 7vw;
  text-align: left;
  margin-right: 36vw;
}

.footer{
  font-family:Cambria, Cochin, Georgia, Times, 'Times New Roman', serif ;
  text-align: center;
  margin-top: 7vh;
  font-size: 60%;
}

.footer h4{
  font-family: 'Righteous', cursive;
}
</style>
