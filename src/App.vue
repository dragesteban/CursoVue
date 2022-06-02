<template>
  <div class="">
    <h1>{{inputText}}</h1>
    <h2 :class="clasePruebas" v-text="texto"></h2>
    <p v-html="textoHtml"></p>
    <input type="text" v-model="inputText">
    <img :src="img" alt="">
  </div>
</template>
<script>
export default {
  name: 'App',
  data () {
    return {
      mensaje: "Hola Vue !",
      texto: "Hola mundo",
      textoHtml: '<a href="https://google.com"> Otra frase </a>',
      inputText: "Escribe un texto",
      img: "https://picsum.photos/300/300",
      clasePruebas: "texto-rojo"
    }
  },
}
</script>
<style>
.texto-azul{
  color:blue;
}
.texto-rojo{
  color:red;
  background-color:black;
}
</style>
