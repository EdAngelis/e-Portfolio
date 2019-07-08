<template lang="pug"> 
  v-container.pa-0(fluid)
    v-toolbar#vtoolbar(block dark app )
      v-toolbar-title e-Portfolio
    v-layout#head.mt-5(row align-center)
      v-flex(xs4)
        h1 Ed Angelis R. Ribeiro
      v-flex.pa-5(xs8 class="text-xs-center")
        p conheci o mundo da programação um pouco tarde, fui apresentado neste mundo apenas quando decidi fazer faculdade, fiquei fascinado desde o princípio, e apesar de ter entrado tarde neste mundo, acredito que minhas experiências de vida até aqui me ajudam muito a me tornar um programador melhor. 
    v-layout(justify-center)
      v-flex(xs6)
        v-card#card
          v-img(:src='src')
          v-card-title(primary-title) E-Commerce Front-End Angular e Bootstrap, Back-End: Node js, MongoDB
      
        
</template>

<script>
import timeline from '../components/timeline'
  export default {

    name: "Home",
    components: {
      timeline
    },
    data () {
      return {
        src: require('@/assets/img/camisateca.jpg')
      }
    }
  }
</script>

<style scoped>
  #vtoolbar {
    border-bottom: 2px solid;
    border-color: yellow;
  }
  #head{
    height: 150px;
    background-color: rgb(224, 224, 224)
  }
  #head h1 {
    position: relative;
    left: 20%;
    size: 200px;
    font-family: 'kalam', cursive

  }
  #head p {
    font-family: 'kalam', cursive
  }
  #card{
  }
</style>

