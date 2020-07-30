<template>
  <div>
    <div class="card">
      <div class="card-image">
        <figure class="image">
          <img src="../../../static/img/Pandemic1.png" alt="Pandemic" />
        </figure>
      </div>
      <div class="card-content">
        <div class="media">
          <div class="media-content">
            <p class="title is-4">Pandemic</p>
          </div>
        </div>

        <div class="content">A 3D game project on Unity written on C#</div>
      </div>
      <footer class="card-footer">
        <button class="card-footer-item button" @click="showPandemicModal">See more</button>
      </footer>
    </div>

    <!-- Modal -->
    <div :class="pandemicModalActive ? 'modal is-active' : 'modal'">
      <div class="modal-background"></div>
      <div class="modal-card">
        <header class="modal-card-head">
          <p class="modal-card-title">Pandemic</p>
          <button class="delete" aria-label="close" @click="hidePandemicModal"></button>
        </header>
        <section class="modal-card-body">
          <!-- Content ... -->
          <p>
            This is a 3D game project me and my friend made when we
            finished a Game Development course at Camosun. The game
            was inspirated by the COVID-19 pandemic in 2020. Player
            will roleplay a police officer going around the city
            and shoots facemasks to patients in order to cure them and
            prevent the virus from spreading to the community.
          </p>
          <br />
          <img class="has-margin-bottom" alt="Pandemic 1" src="../../../static/img/Pandemic1.png" />
          <div class="divider" />
          <img class="has-margin-bottom" alt="Pandemic 2" src="../../../static/img/Pandemic2.png" />
        </section>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Pandemic",
  data() {
    return {
      pandemicModalActive: false,
    };
  },
  methods: {
    showCapstoneModal: function () {
      this.pandemicModalActive = true;
    },
    hideCapstoneModal: function () {
      this.pandemicModalActive = false;
    },
  },
};
</script>

<style scoped>
</style>