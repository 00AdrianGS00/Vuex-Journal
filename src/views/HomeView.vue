<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <button @click="goToDayBook" class="btn btn-primary">primary</button>
    <button class="btn btn-secondary">secondary</button>
    <button class="btn btn-success">danger</button>
  </div>
</template>

<script>
export default {
  methods: {
    goToDayBook() {
      this.$router.push( {name: 'daybook' })
    }
  }
}
</script>