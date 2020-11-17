<template>
  <div>
    <counter v-if="cazzo" :name="name" />
  </div>
</template>
<script>
import counter from '../components/counter'

export default {
  components: {
    counter
  },
  /*
  async asyncData () {
    await ----
    return null
  },
  */
  data () {
    return {
      name: 'ZZZ',
      cazzaccio: true
    }
  },
  computed: {
    cazzo () {
      return this.cazzaccio
    }
  },
  methods: {
  }
}
</script>
