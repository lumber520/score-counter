<template>

  <ScoreCounter name="Player 1" />
<ScoreCounter name="Player 2" />
</template>

<script setup>
  import ScoreCounter from "./components/ScoreCounter";
  export default {
    components: {ScoreCounter}
  }
</script>

<style>
#app {
  font-family:  sans-serif;
  font-size: 3em;
  text-align: center;
  color: #2c3e50;
}
</style>
