<template>
<NavBar :alt="appname" :logo="logo" />
<router-view />
<Footer />
</template>

<script>
import NavBar from './components/NavBar.vue';
import Footer from './components/Footer.vue';
export default {
components:{
  NavBar,
  Footer
},
data(){
return{
  appname:"MakeYourBurguer",
  logo:"/img/logo.png"
}
}
}
</script>

<style>
*{
  font-family: Helvetica,;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body{
  width: 100%;
  height: 100vh;
}
.mainContainer{
  margin: 50px;
  min-height: 500px;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
h1{
  display: block;
  text-align: center;
  font-size: 42px;
  margin-bottom: 30px;
  color: #222;
}

</style>