<template>
  <div id="app">
    <h1>Форма создания клиента</h1>
    <hr>
    <FormAuth />

   
  </div>
</template>

<script>

import FormAuth from '@/components/FormAuth'
export default {
  name: 'App',
  components: {
    FormAuth
   
  }
}
</script>

<style lang="sass">
#app
  font-family: Avenir, Helvetica, Arial, sans-serif
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
  text-align: center
  color: #435970
  margin-top: 60px

</style>
