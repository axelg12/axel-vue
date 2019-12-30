<template>
  <v-app :style="{ background: 'rgb(255, 225, 187)' }">
    <div id="app">
      <List />
    </div>
  </v-app>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import List from "./components/List.vue";

@Component({
  components: {
    List
  }
})
export default class App extends Vue {}
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  flex-direction: column;
  text-align: center;
  color: #2c3e50;
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
