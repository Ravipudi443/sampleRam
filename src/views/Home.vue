<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <h4>You have been redirected to Home</h4>
    <h4><router-link to="/about">Go back</router-link></h4>
    <h4><router-link to="/">Go to Landing</router-link></h4>
  </div>
</template>

<script>
// @ is an alias to /src


export default {
  name: 'Home',
  components: {
    
  }
}
</script>
