<template>
  <div class="popup">
    <component :is="$props.type" v-bind="$props"></component>
  </div>
</template>

<script>
import EditorA from "./EditorA.vue";
import EditorB from "./EditorB.vue";

export default {
  components: {
    EditorA,
    EditorB,
  },
  props: {
    type: {
      type: String,
      default: "EditorA"
    },
    data: {
      type: Object,
      default: () => ({})
    }
  },
}
</script>

<style lang="css" scoped>
.popup {
  border: 1px solid red;
  min-height: 200px;
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: center;
  align-content: stretch;
  align-items: center;
}
</style>