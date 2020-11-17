<template>
  <div>
    Ciao {{name}} --- {{teo}} --- {{teodue}}
    <div @click="add">Add</div>
    <div @click="clear">Clear</div>
  </div>
</template>
<script>
export default {
  props: {
    name: {
      type: String,
      default: 'Ciccio'
    }
  },
  data () {
    return { teo: 1 }
  },
  computed: {
    teodue () {
      return this.teo * 2
    }
  },
  methods: {
    add () {
      this.teo += 1
    },
    clear () {
      this.teo = 1
    }
  }
}
</script>
<style scoped>

</style>
