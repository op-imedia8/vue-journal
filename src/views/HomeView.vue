<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <h1>Hola Mundo</h1>

    <button class="btn btn-primary" @click="goToDaybook">primary</button>
    <button class="btn btn-secondary" @click="goToDaybook">secondary</button>
    <button class="btn btn-success" @click="goToDaybook">success</button>
  </div>
</template>

<script>
// @ is an alias to /src


export default {
  name: 'HomeView',
  components: {
   
  },
  methods:{
    goToDaybook(){
      this.$router.push({name:'no-entry'})
    }
  }
}
</script>
