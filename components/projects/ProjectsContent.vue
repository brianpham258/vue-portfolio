<template>
  <div>
    <div id="projects" class="is-background-primary is-title">PROJECTS</div>
    <div class="columns is-desktop">
      <div class="column">
        <Capstone />
      </div>
      <div class="column">
        <PizzaPalace />
      </div>
      <div class="column">
        <TukTukHeaven />
      </div>
    </div>
    <div class="columns is-desktop">
      <div class="column">
        <Pandemic />
      </div>
      <div class="column">
        <GameJam />
      </div>
      <div class="column" />
    </div>
  </div>
</template>

<script>
import Capstone from "./projects/Capstone.vue";
import PizzaPalace from "./projects/PizzaPalace.vue";
import TukTukHeaven from "./projects/TukTukHeaven.vue";
import GameJam from "./projects/GameJam.vue";
import Pandemic from "./projects/Pandemic.vue";

export default {
  name: "ProjectContent",
  components: {
    Capstone,
    PizzaPalace,
    TukTukHeaven,
    GameJam,
    Pandemic,
  },
};
</script>

<style scoped>
</style>