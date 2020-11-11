<template>
  <div id="sample01">
      <h1>Hello {{ name }}</h1>
      <input type="text" :value="name">
  </div>
</template>

<script>
export default {
    name: "sample01",
    data() {
        setInterval(() => {
            this.name +=  1
        }, 1000);
        return {
            name: 0,
        }
    },
}
</script>

<style>

</style>