<template>
  <div class="card" @click="showImg">
    <img 
      src="../assets/RussellMNelson.jpg"
      v-show="boolImg"
    >
  </div>
</template>

<script>
export default {
  name: "MemoryCard",
  props: {

  },
  data() {
    return {
      imgVisibility: false
    }
  },
  methods: {
    showImg() {
      this.imgVisibility = !this.imgVisibility
    }
  },
  computed: {
    boolImg() {
      return this.imgVisibility
    }
  }
}
</script>

<style scoped>
  .card {
    background-color: rgb(105, 105, 105);
    padding: 5px;
    margin: auto;
    margin-bottom: 1em;
    height: 10em;
    width: 10em;
    border-radius: 20px;
  }
  .card img {
    border-radius: 20px;
    height: 10em;
  }
</style>