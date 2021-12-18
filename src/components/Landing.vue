<template>
<div class="container">
  <div class="business-logo">
    <div class="business-logo--main">
      <img alt="business logo" src="../assets/business-logo.png">

    </div>
    <div class="business-logo--ballons">
     <img src="../assets/ballons.png" alt="ballons">
    </div>
  </div>
  <div class="login-button">
    <img src="../assets/login-icon.png" alt="login button">
  </div>
  <div class="footer">
    <footer>
      <h4>Powered By</h4>
      <h4>My Invites</h4>
    </footer>
  </div>
</div>
</template>

<script>
export default {
  name: 'Landing',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container{
  height: 100%;
  background-image: url('../assets/background.png');
  background-repeat: no-repeat;
  background-size: cover;
}
@media only screen and (min-width: 375px){
    .container{
      height:100%;
    }
}

.business-logo{
  display: flex;
  justify-content: space-between;
}
@media only screen and (min-width: 375px){
  .business-logo{
    display: flex;
    align-items: center;
    justify-content: end;
  }
  .business-logo--main{
    margin-right:-100px;
  }
}

@media only screen and (min-width: 1024px){
  .business-logo{
  display: flex;
  justify-content: space-between;
}
}

.login-button{
  margin-top: 35px;
  display: flex;
  justify-content: center;
}

.footer{
  display: flex;
  justify-content: center;
}

@media only screen and (min-width: 375px) {
  .footer{
    margin-top: 18%;
  }
}

@media screen and (min-width: 1024px) {
  .footer{
    margin-top: 6%;
  }
}

footer{
  display: flex;
  flex-direction: column;
}
  
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
