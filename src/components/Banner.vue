<template>
  <div id="banner">
    <h1>Make Your Burguer</h1>
  </div>
</template>

<script>
export default {
name:"Banner"
}
</script>

<style scoped>
#banner h1{
color: #fff;
margin: 20px;
background-color: #222;
padding: 20px 40px;
border-radius: 12px;
}
#banner{
    background-image: url("/public/img/burger.jpg");
    background-position:0 -250px ;
    background-size: cover;
    display: flex;
    height: 600px;
    justify-content: flex-start;
    align-items: center;

}
</style>