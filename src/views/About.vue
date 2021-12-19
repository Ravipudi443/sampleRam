<template>
  <div class="about">
    <h1>This is an about page</h1>
    <h4><router-link to="/">Go back</router-link></h4>
    <h4><router-link to="/home">Go Home</router-link></h4>
  </div>
</template>
<script>
export default {
   name: 'About',
   methods:{
   goToHome(){
   this.$router.push('/'); 
      }
  }
}
</script>
