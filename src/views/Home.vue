<template>
  <div class="wrapper">
    <div class="search">
      <input id="search" name="search" />
      <label for="search">Search</label>
    </div>
  </div>
</template>

<script>
export default {
  name: 'home'};
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
  width: 300px;
}
input {
  height: 50px;
  border: 0;
  border-bottom: 1px solid black;
}
</style>
