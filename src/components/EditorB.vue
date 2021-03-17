<template>
  <div>
    EditorB: {{ val }}  {{ bprop }}
  </div>
</template>

<script>
export default {
  props: {
    data: {
      type: Object,
      default: () => ({})
    },
    bprop: String,
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