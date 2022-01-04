<script>
import Menu from './components/Menu.vue'
import PageContent from './components/PageContent.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Menu,
    PageContent,
    Footer
  }
}
</script>

<template>
<div>
  <Menu/>

  <PageContent text="Bonjour je m'appelle Maxence." numero="1"/>
  <PageContent text="Je recherche une alternance" numero="2"/>
  <PageContent text="dans le domaine du marketing" numero="3"/>
  <PageContent text="contact@maxence.fr" numero="4"/>

  <Footer/>
</div>
  
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
