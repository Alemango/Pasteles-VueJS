<template>
    <div>
        <button class="botonMorado">{{ texto }}</button>
    </div>
</template>

<script>
export default {
    name: 'botonMorado',
    props: {
        texto: String
    }
}
</script>

<style scoped>
.botonMorado {
    font-size:90%;
    font-family:'Righteous', cursive;
    width:11vw;
    height:8vh;
    border-width:2px;
    color:#bc80ea;
    border-color:#c584f3;
    font-weight:bold;
    border-radius: 6px;
    box-shadow:inset 0px 1px 0px 0px #efdcfb;
    text-shadow:inset 0px 1px 0px #9752cc;
    background:#dfbdfa;
}
  
.botonMorado:hover {
    background: #bc80ea;
    color: rgb(214, 205, 205);
}
</style>