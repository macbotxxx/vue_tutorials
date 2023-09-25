<script setup>
let count = 0;

const addToCount = () => {
  count = count + 1;
}

const subtractCount = () => {
  
  count = count - 1;
}

</script>

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