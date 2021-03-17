<template>
  <div id="app">
    <Popup @click.native="changeType" :type="editorType" :data="{ a: 1, b: 2 }" />
  </div>
</template>

<script>
import Popup from './components/Popup';

export default {
  name: 'App',
  components: {
    Popup,
  },
  data() {
    return {
      editorType: "EditorB",
    }
  },
  methods: {
    changeType() {
      if (this.editorType === "EditorA") {
        this.editorType = "EditorB";
      } else {
        this.editorType = "EditorA";
      }
    }
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
