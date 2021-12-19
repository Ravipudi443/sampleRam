<template>
<div id="landing">
<div id="section">
  <b-col>
  <b-row align-h="between" class="logo">
    <b-col cols="2" class="business-logo">
      <img src="../assets/business-logo.png" alt="business-logo">
    </b-col>
    <b-col cols="3"  class="business-ballons">
      <img src="../assets/ballons.png" alt="ballons">
    </b-col>
  </b-row>
  
  <div class="button-group">
    <div class="button-group--row">
      
        <b-button class="login-button" size="lg"  @click="goToHome()">LOGIN</b-button>
      
        <b-button class="login-button--info" size="lg"><img src="../assets/Vector.png" alt="info-logo"> </b-button>
     
    </div>
  </div>
  <footer>
  <div class="footer-text">
    <h4>Powered by</h4>
    <h4>My Invites</h4>
  </div>
  </footer>
  </b-col>
</div>
</div>
</template>

<script>
export default {
  name: 'Landing',
  props: {
    msg: String
  },
  methods:{
   goToHome(){
   this.$router.push('/about'); 
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#landing{
  background-image: url('../assets/background.png');
  background-repeat: no-repeat;
  background-size: cover;
}
.section{
  /* background-image: url('../assets/background.png');
  background-repeat: no-repeat;
  background-size: cover; */
  height: 100vh;
}
.login-button{
background: linear-gradient(90deg, rgba(30, 98, 164, 0.522) 0%, rgba(31, 96, 161, 0.9) 0%, rgba(54, 194, 239, 0.9) 53.68%, rgba(30, 98, 164, 0.9) 100%);
background-blend-mode: darken;
width:100%;
border-radius: 10px 0px 0px 10px;
}
.login-button--info{
background: linear-gradient(90deg, rgba(30, 98, 164, 0.522) 0%, rgba(31, 96, 161, 0.9) 0%, rgba(54, 194, 239, 0.9) 53.68%, rgba(30, 98, 164, 0.9) 100%);
background-blend-mode: darken;
border-radius: 0px 10px 10px 0px;
}
.button-group{
  display: flex;
  justify-content: center;
}
.button-group--row{
  display: flex;
  width: 33%;
}
footer{
  display: flex;
  justify-content: center;
  margin-top: 6%;
}
.footer-text{
font-family: Roboto;
font-style: normal;
font-weight: normal;
font-size: 16px;
line-height: 30px;
text-align: center;
letter-spacing: -0.5px;
color: #606D79;
}
.router-link{
  text-decoration: none;
}
</style>
