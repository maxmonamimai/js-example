<template>
  <div id="sample03">
      <h1>Hello {{ name }}</h1>
      <br>
      <h2>{{ upperName }}</h2>
      <h2>{{ saraly }}</h2>
      <h2>{{ tax }}</h2>

      <input type="text" :value="name">
      <br>
      <input type="text" v-model="name">
  </div>
</template>

<script>
export default {
    name: "sample01",
    data() {
        return {
            name: 'mc CHakkPong',
            saraly: 500001,
        }
    },
    computed: {
        upperName() {
            return this.name.toUpperCase()
        },
    },
}
</script>

<style>

</style>