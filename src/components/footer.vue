<template>
  <div id="footer">
    <div class="settings">
      <img class="random" @click="randomAvatar()" :src="require('../assets/img/random.svg')">

      <img class="random" @click="clearAvatar()" :src="require('../assets/img/clear.svg')">

      <SaveImage/>
    </div>

    <Options />

  </div>
</template>

<script>
import Options   from './options'

// import save Image
import SaveImage from './save_image'

export default {
  name: "Footer",
  components: {
    Options,
    SaveImage
  },
  methods: {
    randomAvatar() {
      this.$root.$refs.Options.resetMenu();
      this.$root.$refs.App.randomAvatar();
    },
    clearAvatar(){
      this.$root.$refs.Options.resetMenu();
      this.$root.$refs.App.resetAvatar();
    }
  }
}
</script>