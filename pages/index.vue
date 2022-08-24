<template>
  <!-- #TODO:
      [ ] Criar rota para página que fará ligação com o Firebase com FirebaseUI
      [ ] Criar autenticação com firebase com base na documentação https://firebase.google.com/docs/auth/web/firebaseui?authuser=0
      [ ] Criar card e rota para página que fará login com Firebase UI personalizada 
  -->
  <div id="main__body">
    <h1 class="main__title">Login com Firebase</h1>
    <Card upper-tag="Login com Firebase" title="Google UI"
      subtitle="Aqui é implementado o Firebase utilizando o UI da google (FirebaseUI)" button-text="Ir para login" />


  </div>
</template>

<script>
import Card from '../components/Card.vue'

export default {
  name: 'IndexPage',
  components: { Card }
}
</script>

<style>
#main__body {
  padding: 4%;
}

.main__title {
  text-align: center;
  font-size: 2.5rem;
  padding: 2.5rem;
}
</style>
