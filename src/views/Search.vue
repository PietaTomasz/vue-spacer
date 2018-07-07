<template>
  <div class="wrapper">
    <div class="search">
    <label for="search">Search</label>
    <input id="search" name="search" v-model="searchValue" @input="handleInput" />      
    </div>
  </div>
</template>

<script>
const API = `https://images-api.nasa.gov`;

export default {
  name: 'Search',
  data() {
      return {
          searchValue: '',
    }
  },
  methods: {
      handleInput(e) {
          console.log(e.target.value);
          console.log(this.searchValue);
      }
  }
};
</script>

<style lang="scss" scoped>
.wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 0;
  padding: 30px;
  width: 100%;
}
.search {
  display: flex;
  flex-direction: column;
  width: 200px;
     
  label {
    font-family: Montserrat, sans-serif;
    text-align: center;
  }
}
input {
  height: 30px;
  border: 0;
  border-bottom: 1px solid black;
  text-align: center;
  font-size: 1.1rem; 
}
</style>
