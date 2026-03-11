<template>
<div id="nav">
        <router-link to="/" id="logo">
       <img :src="logo" :alt="alt">
    </router-link>
    <router-link to="/">
        Home
    </router-link>
        <router-link to="/pedidos">
        Pedidos
    </router-link>
</div>
</template>

<script>
export default {
name:"NavBar",
props:[
    "logo",
    "alt",
]
}
</script>

<style scope>
#nav{
    background-color:#222;
    border-bottom: 4px solid #111;
    padding: 15px 50px;
    display: flex;
    justify-content: flex-end;
    align-items: center;
}

img{
  width: 40px;
  height: 40px;
}
#nav #logo{
      margin: auto;
  margin-left: 0px;
}
#nav a{
    color: #FCBA03;
    text-decoration: none;
    transition: 0,9s;
    margin: 12px;
}
#nav a:hover{
    color: #fff;
}
</style>