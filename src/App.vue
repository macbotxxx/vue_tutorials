<script setup>
  import { ref } from 'vue'

  const count = ref(0);

  const addToCount = () => {
    count.value = count.value + 1;
  }
 
  const subtractCount = () => {
    count.value = count.value - 1;
  }

</script> 

<!-- <script >
  export default({
    data(){
      return{
        count : 0
      }
    }
  })
</script> -->

<template>
  <main>
    <div>
      <h1>Counter</h1>
      <h1>{{ count  }}</h1>
      <button @click="subtractCount()"> - </button>
      <button @click="addToCount()"> + </button>
  
    </div>
  </main>
</template>

<style scope>

main {
  background-color: bisque;
  width: 100vw;
  height: 100vh;
  display:flex;
  align-items: center;
  justify-content: center;
}

div {
  text-align: center;
}

</style>