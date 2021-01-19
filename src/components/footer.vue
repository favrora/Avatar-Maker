<template>
  <div id="footer">
    <div id="settings">
      <img id="random" @click="reloadPage()" :src="require('../assets/img/random.svg')">
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
    reloadPage() {
      window.location.reload()
    }
  }
}
</script>