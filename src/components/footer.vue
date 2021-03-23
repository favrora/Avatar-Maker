<template>
  <div id="footer">
    <div id="settings">
      <img id="random" @click="randomAvatar()" :src="require('../assets/img/random.svg')">
    </div>
    <div id="settings">
      <img id="random" @click="clearAvatar()" :src="require('../assets/img/clear.svg')">
    </div>

    <Options />

  </div>
</template>

<script>
import Options from './options'

export default {
  name: "Footer",
  components: {
    Options
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