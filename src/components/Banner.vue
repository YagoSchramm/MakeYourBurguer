<template>
  <div class="banner">
    <h1 class="bannerh1">Make Your Burguer</h1>
  </div>
</template>

<script>
import gsap from 'gsap';
export default {
name:"Banner",
mounted(){
const tl=gsap.timeline()
tl.from(".banner",{
  y:-50,
  opacity:0,
  duration:0.5
});
tl.from(".bannerh1",{
  x:-100,
  opacity:0.0,
  duration:0.5
},"+=1")

}
}
</script>

<style scoped>
.bannerh1{
color: #fff;
margin: 20px;
background-color: #222;
padding: 20px 40px;
border-radius: 12px;
}
.banner{
    background-image: url("/public/img/burger.jpg");
    background-position:0 -250px ;
    background-size: cover;
    display: flex;
    height: 600px;
    justify-content: flex-start;
    align-items: center;

}
</style>