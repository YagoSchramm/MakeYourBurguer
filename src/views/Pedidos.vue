<template>
         <h1>Gerenciar Pedidos:</h1>  
      <div class="mainContainer">
 
        <Dashboard/>
  </div>
</template>

<script>
import Dashboard from '@/components/dashboard.vue';

export default {
name:"Pedidos",
components:{
Dashboard
}
}
</script>

<style scope>
.mainContainer{
  display: flex;
  justify-content: center;
 
}
h1{
  margin-top: 30px;
}

</style>