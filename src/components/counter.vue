
<template>

   <main class="main" id="app">
  <h1>Counter Exercise</h1>
  <article class="counter">
    <h2 v-if="amount%2==0">The count is even</h2>
    <h2 v-else>The count is odd</h2>
    <p class="count">{{amount}}</p>
    <button v-on:click="increment()">Increment by 1</button> <!-- goes up one-->
    <button v-on:click="decrement()">Decrement by 1</button> <!-- goes down one-->
    <button v-on:click="reset()">Reset</button>
    <div class="input-group">
      <label for="amount">Amount</label>
      <input type="number"  v-model.number = "amount">
    </div>
  </article>
</main>
</template>

<script>
export default {
    data(){  // retuned
      return {
        amount:0
      }
    },

    methods: {
      increment(){ //add one
        this.amount+=1;
      },

      decrement(){
        this.amount-=1; //down one 
      },

      reset(){  //reset 
        this.amount=0;
      }
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



