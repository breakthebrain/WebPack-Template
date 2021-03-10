<template>
  <section id="main">
    <div class="container">
      <img src="/assets/img/logo.png" :alt="message">
      <h1>{{message}}</h1>
    </div>
  </section> 
</template>

<script>
export default {
  data() {
    return {
      message: null,
    }
  },
  created() {
    this.message = this.$store.getters.getMessage 
  }
};
</script>

<style lang="scss">
  h1 {
    color: green;
  }
</style>