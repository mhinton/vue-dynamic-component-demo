<template>
  <div>
    EditorB: {{ val }}
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
      return this.data.b; 
    }
  },
}
</script>

<style lang="css" scoped>

</style>