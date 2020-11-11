<template>
  <div id="sample01">
      <h1>Hello {{ name }}</h1>
      <input type="text" :value="name">
      <br>
      <input type="text" v-model="name">
  </div>
</template>

<script>
export default {
    name: "sample01",
    data() {
        setInterval(() => {
            this.name +=  1
        }, 3000);
        return {
            name: 0,
        }
    },
}
</script>

<style>

</style>