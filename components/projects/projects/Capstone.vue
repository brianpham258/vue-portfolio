<template>
  <div>
    <div class="card">
      <div class="card-image">
        <figure class="image">
          <img src="../../../static/img/CapstoneHome.png" alt="Capstone" />
        </figure>
      </div>
      <div class="card-content">
        <div class="media">
          <div class="media-content">
            <p class="title is-4">Capstone project</p>
          </div>
        </div>

        <div class="content">A web application that uses for managing videos</div>
      </div>
      <footer class="card-footer">
        <button class="card-footer-item button" @click="showCapstoneModal">See more</button>
      </footer>
    </div>

    <!-- Modal -->
    <div :class="capstoneModalActive ? 'modal is-active' : 'modal'">
      <div class="modal-background"></div>
      <div class="modal-card">
        <header class="modal-card-head">
          <p class="modal-card-title">Capstone Project</p>
          <button class="delete" aria-label="close" @click="hideCapstoneModal"></button>
        </header>
        <section class="modal-card-body">
          <!-- Content ... -->
          <p>
            This is my capstone project, which me and two other
            classmates have just finished on August of 2020.
            This is, so far, my biggest and most professional
            project. In this project, I was responsible for all of
            the front-end tasks.
          </p>
          <br />
          <a
            href="https://portal.witnessblanket.ca/login"
            target="_blank"
            rel="noreferrer"
          >Checkout the website here</a>
          <br />
          <img
            alt="Capstone Home"
            src="../../../static/img/CapstoneHome.png"
            class="has-margin-bottom"
          />
          <div class="divider" />

          <img
            alt="Capstone Video Details"
            src="../../../static/img/CapstoneVideoDetails.png"
            class="has-margin-bottom"
          />
          <div class="divider" />

          <img
            alt="Capstone Playlists"
            src="../../../static/img/CapstonePlaylists.png"
            class="has-margin-bottom"
          />
          <div class="divider" />

          <img
            alt="Capstone Playlist Videos"
            src="../../../static/img/CapstonePlaylistVideos.png"
            class="has-margin-bottom"
          />
          <div class="divider" />

          <img
            alt="Capstone Categories"
            src="../../../static/img/CapstoneCategories.png"
            class="has-margin-bottom"
          />
          <div class="divider" />

          <img
            alt="Capstone Curation"
            src="../../../static/img/CapstoneCuration.png"
            class="has-margin-bottom"
          />
          <div class="divider" />

          <img
            alt="Capstone Users"
            src="../../../static/img/CapstoneUsers.png"
            class="has-margin-bottom"
          />
          <div class="divider" />

          <img
            alt="Capstone Profile"
            src="../../../static/img/CapstoneProfile.png"
            class="has-margin-bottom"
          />
        </section>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Capstone",
  data() {
    return {
      capstoneModalActive: false,
    };
  },
  methods: {
    showCapstoneModal: function () {
      this.capstoneModalActive = true;
    },
    hideCapstoneModal: function () {
      this.capstoneModalActive = false;
    },
  },
};
</script>

<style scoped>
.has-indentation {
  margin-left: 30px;
}
</style>