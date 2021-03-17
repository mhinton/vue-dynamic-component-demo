<template>
  <div>
    EditorA: {{ val }}  {{ aprop }}
  </div>
</template>

<script>
export default {
  props: {
    data: {
      type: Object,
      default: () => ({})
    },
    aprop: String
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