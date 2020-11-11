<template>
  <div id="sample05">
      
      <h2 v-if="ok">{{ upperName }}</h2>

      <h2 v-show="ok">{{ upperName }}</h2>

      

      <input type="text" :value="name">
      <br>

      <input type="text" v-model="name">

    <br>

      <input type="text" v-model="name">

      <button @click="doSave">Save</button>
  </div>
</template>

<script>
export default {
    name: "sample05",
    data() {
        return {
            ok: true,
            name: 'mc CHakkPong',
            saraly: 500001,
        }
    },
    computed: {
        upperName() {
            return this.name.toUpperCase()
        },
    },
    methods: {
        doSave() {
            this.ok = !this.ok
            console.log("Save", this.name, this.uppername);
        },
    },
}
</script>

<style>

</style>