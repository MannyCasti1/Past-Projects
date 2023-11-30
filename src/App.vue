
<template>
<div> 
<counter />  <!-- using templete to migrate my data from componets-->
</div>
</template>


<script>
import counter from './components/counter.vue' // coming from my componte.vue and all it data
export default {
  name: 'App',
  components: {
    counter
  }
}
</script>

<style>

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #1a9b09;
  margin-top: 60px;
}
</style>






    
    
