<template>
  <MyHeader msg="NAVIGATION PANE"/>
  <div class="cards-container">
    <MemoryCard />
    <MemoryCard />
    <MemoryCard />
    <MemoryCard />
    <MemoryCard />
    <MemoryCard />
    <MemoryCard />
    <MemoryCard />
    <MemoryCard />
    <MemoryCard />
    <MemoryCard />
    <MemoryCard />
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MemoryCard from './components/MemoryCard.vue'

export default {
  name: 'App',
  components: {
    MyHeader, MemoryCard
  }
}
</script>

<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #e3e6e9;
    margin-top: 60px;
  }

  .cards-container {
    display: grid;  
    grid-template-columns: 1fr 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr;
    margin: auto;
    max-width: 60%;
  }
</style>
