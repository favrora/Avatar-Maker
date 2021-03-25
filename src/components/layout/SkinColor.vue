<template>
  <svg id="skinColor" width="360px" height="360px" viewBox="0 0 360 360" style="z-index: 80">
    <g id="skin_white" class="show">
      <path fill="#edb98a" d="M304 360l0 -15c0,-47 -39,-85 -86,-85l-8 0 0 -22c22,-10 37,-32 39,-57 7,-1 13,-7 13,-15l0 -15c0,-8 -6,-14 -13,-15l0 -8c0,-38 -31,-69 -69,-69l0 0c-38,0 -69,31 -69,69l0 8c-7,1 -13,7 -13,15l0 15c0,8 6,14 13,15 2,25 17,47 39,57l0 22 -8 0c-47,0 -86,38 -86,85l0 15 248 0z"/>
      <path fill="#000000" fill-opacity="0.2" d="M180 256c-11,0 -21,-2 -30,-6l0 -12c9,5 19,7 30,7l0 0c11,0 21,-2 30,-7l0 12c-9,4 -19,6 -30,6z"/>
      <path fill="#000000" fill-opacity="0.2" d="M180 181c9,0 16,-4 16,-9l-32 0c0,5 7,9 16,9z"/>
    </g>
    <g id="skin_black">
      <path fill="#6c4f34" d="M304 360l0 -15c0,-47 -39,-85 -86,-85l-8 0 0 -22c22,-10 37,-32 39,-57 7,-1 13,-7 13,-15l0 -15c0,-8 -6,-14 -13,-15l0 -8c0,-38 -31,-69 -69,-69l0 0c-38,0 -69,31 -69,69l0 8c-7,1 -13,7 -13,15l0 15c0,8 6,14 13,15 2,25 17,47 39,57l0 22 -8 0c-47,0 -86,38 -86,85l0 15 248 0z"/>
      <path fill="#000000" fill-opacity="0.2" d="M180 256c-11,0 -21,-2 -30,-6l0 -12c9,5 19,7 30,7l0 0c11,0 21,-2 30,-7l0 12c-9,4 -19,6 -30,6z"/>
      <path fill="#000000" fill-opacity="0.2" d="M180 181c9,0 16,-4 16,-9l-32 0c0,5 7,9 16,9z"/>
    </g>
  </svg>
</template>

<script>
export default {
  name: "SkinColor",
  data() {
    return {
      list: ['#skin_white','#skin_black']
    }
  },

  methods: {
    picker(option = false) {
      this.hide_all();
      option
        ? document.querySelector(option).classList.add('show')
        : document.querySelector(this.random_option()).classList.add('show');
    },
    random_option() {
      var chosenSkinColor = Math.floor(Math.random() * this.list.length);
      return this.list[chosenSkinColor];
    },
    hide_all() {
      for (let i = 0; i < this.list.length; i++) {
        document.querySelector(this.list[i]).classList.remove('show');
      }
    }
  },

  created() {
    this.$root.$refs.SkinColor = this;
  }
}
</script>