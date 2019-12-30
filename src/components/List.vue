<template>
  <div class="container">
    <div class="List">
      <div
        v-bind:class="{ active: selectedBlock === 'about' }"
        v-on:click="onChange('about')"
        class="item item__about"
      />
      <div
        v-bind:class="{ active: selectedBlock === 'school' }"
        v-on:click="onChange('school')"
        class="item item__pantheon"
      />
      <div
        v-bind:class="{ active: selectedBlock === 'work' }"
        v-on:click="onChange('work')"
        class="item item__work"
      />
    </div>
    <transition name="List__fade" mode="out-in">
      <div
        class="List__description"
        v-if="selectedBlock === 'school'"
        key="school"
      >
        <Academic />
      </div>
      <div
        class="List__description"
        v-if="selectedBlock === 'about'"
        key="about"
      >
        <Me />
      </div>
      <div class="List__description" v-if="selectedBlock === 'work'" key="work">
        <Work />
      </div>
    </transition>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";
import Academic from "./Academic.vue";
import Me from "./Me.vue";
import Work from "./Work.vue";

@Component({
  components: {
    Academic,
    Me,
    Work
  }
})
export default class List extends Vue {
  selectedBlock: string = "about";
  onChange(selected: string) {
    this.selectedBlock = selected;
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.List {
  margin-top: 20px;
  display: flex;
  flex-direction: row;
  justify-content: center;
}
.List__fade-enter-active,
.List__fade-leave-active {
  transition: opacity 0.5s;
}
.List__fade-enter, .List__fade-leave-to /* .List__fade-leave-active below version 2.1.8 */ {
  opacity: 0;
}
.active {
  border: 2px solid #fff;
  border-radius: 3px;
}
.container {
  position: relative;
  width: 1198px;
  padding: 0;
}
.List__description {
  position: absolute;
  top: 100px;
  width: 100%;
}
.item {
  margin-right: 10px;
  height: 50px;
  width: 50px;
}
.item__about {
  background: url("../assets/aboutme.svg");
  background-size: contain;
}
.item__pantheon {
  background: url("../assets/building.svg");
  background-size: contain;
}
.item__work {
  background: url("../assets/work.svg");
  background-size: contain;
}
</style>
