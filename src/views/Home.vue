<template lang="pug"> 
  v-container.body.pa-0(fluid)
    v-toolbar#vtoolbar(block dark app )
      v-toolbar-title e-Portfolio
    v-layout#head.mt-5(row wrap align-center)
      v-flex(lg4 md4 xs12)
        h1.text-xs-center Ed Angelis R. Ribeiro
      v-flex.pa-5(lg8 md8 xs12 class="text-xs-center")
        p conheci o mundo da programação um pouco tarde, fui apresentado neste mundo apenas quando decidi fazer faculdade, fiquei fascinado desde o princípio, e apesar de ter entrado tarde neste mundo, acredito que minhas experiências de vida até aqui me ajudam muito a me tornar um programador melhor. 
    v-layout(justify-center)
      v-flex.mt-3(xs6)
        v-card.card.pb-3(color="rgb(224, 224, 224)")
          a(href="https://camateca.000webhostapp.com" target="_blank")
            v-img.cardImg(:src='src' href="https://camateca.000webhostapp.com")
          v-layout(align-center column)  
            v-card-title.title-card.display-1.font-weight-black.pa-1 E-Commerce
            v-card-subheader Html, Css, JavaScript, BootStrap, Nodejs, MongoDB
            v-divider
            v-card-actions
              a(href="https://github.com/EdAngelis/portal" target="_blank") https://github.com/EdAngelis/portal
          ul 
            li Sistema de Cadastro e Login com Criptografia e Token, com validação no Front e no Back
            li Carrinho de Compras e api de Pagamento Cielo, com pagamentos em cartão de crédito e débito habilitados.
            li Fale conosco, envio de mensagens para o admin usando Node-Mailer.


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
  .body {
    height: 1000px;
    background-color: rgb(88, 88, 88)
  }
  #vtoolbar {
    border-bottom: 2px solid;
    border-color: yellow;
  }
  #head{
    background-color: rgb(224, 224, 224)
  }
  #head h1 {
    size: 200px;
    font-family: 'kalam', cursive

  }
  #head p {
    font-family: 'kalam', cursive
  }
  .card{
    border-radius: 20px;
    
  }
  .cardImg{
    border-radius: 20px;
    height: 300px;
  }

</style>

