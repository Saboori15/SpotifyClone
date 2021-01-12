<template>
  <div class="home">
    <div class="grid grid-cols-12">
      <div class=" col-span-3 side-menu">
        <div class="side-menu-upper-row row-span-11">
          <div class="side-logo-logo m-8">Spotify</div>
          <div class="side-logo-upper m-4">
            <ul>
              <li>Home</li>
              <li>Search</li>
              <li>Your library</li>
            </ul>
          </div>
          <div class="playlist m-4">
            <h4>Playlist</h4>
            <ul>
              <li>Create Playlist</li>
              <li>Liked Songs</li>
            </ul>
          </div>
        </div>

        <div class="privacy row-span-1">
          <ul>
            <li>Cookies</li>
            <li>Privacy</li>
          </ul>
        </div>
      </div>
      <div class="grid grid-rows-7 col-span-9 dashboard">
        <div class="upper-dashboard row-span-1 grid grid-cols-12">
          <div class="skips col-span-9 flex space-x-4 m-4">
            <h1>left</h1>
            <h1>right</h1>
          </div>
          <div class="sign-login col-span-3 flex space-x-4 m-4">
            <h1>signin</h1>
            <h1>login</h1>
          </div>
        </div>
        <div class="playlist row-span-6">
          <div class="each-playlist grid grid-rows-4">
            <Playlist />
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="player">
    <div class="dashboard">Player</div>
  </div>
</template>

<script>
import Playlist from "./Playlist.vue";
export default {
  components: {
    Playlist: Playlist
  }
};
</script>

<style scoped>
.home {
  height: 90vh;
}

.player {
  height: 10vh;
}
.side-menu {
  height: 90vh;
}
.upper-dashboard {
  height: 3em;
}
</style>
