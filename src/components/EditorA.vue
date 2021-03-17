<template>
  <div>
    EditorA: {{ val }}
  </div>
</template>

<script>
export default {
  props: {
    data: {
      type: Object,
      default: () => ({})
    },
  },
  computed: {
    val() {
      return this.data.a; 
    }
  },
}
</script>

<style lang="css" scoped>

</style>