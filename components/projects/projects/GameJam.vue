<template>
  <div>
    <div class="card">
      <div class="card-image">
        <figure class="image">
          <img src="../../../static/img/GameJam2.png" alt="GameJam" />
        </figure>
      </div>
      <div class="card-content">
        <div class="media">
          <div class="media-content">
            <p class="title is-4">Global GameJam 2019</p>
          </div>
        </div>

        <div class="content">A small 2D game project on Unity written on C#</div>
      </div>
      <footer class="card-footer">
        <button class="card-footer-item button" @click="showGameJamModal">See more</button>
      </footer>
    </div>

    <!-- Modal -->
    <div :class="gamejamModalActive ? 'modal is-active' : 'modal'">
      <div class="modal-background"></div>
      <div class="modal-card">
        <header class="modal-card-head">
          <p class="modal-card-title">Global GameJam 2019</p>
          <button class="delete" aria-label="close" @click="hideGameJamModal"></button>
        </header>
        <section class="modal-card-body">
          <!-- Content ... -->
          <p>
            This is a 2D game project me and my friend made while
            taking part in the Global Game Jam 2019 event. The game
            was about a dog got lost and had to find his way to home.
          </p>
          <br />
          <img class="has-margin-bottom" alt="Game Jam 1" src="../../../static/img/GameJam1.png" />
          <div class="divider" />
          <img class="has-margin-bottom" alt="Game Jam 2" src="../../../static/img/GameJam2.png" />
          <div class="divider" />
          <img class="has-margin-bottom" alt="Game Jam 3r" src="../../../static/img/GameJam3.png" />
        </section>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "GameJam",
  data() {
    return {
      gamejamModalActive: false,
    };
  },
  methods: {
    showGameJamModal: function () {
      this.gamejamModalActive = true;
    },
    hideGameJamModal: function () {
      this.gamejamModalActive = false;
    },
  },
};
</script>

<style scoped>
</style>