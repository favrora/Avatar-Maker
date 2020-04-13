<template>

<div class="mn">

  <div @click="showBlazer()">
    <svg viewBox="0 0 280 280">
     <g id="c_blazer">
      <path class="tinted" fill="#545454" d="M264 280l0 -13c0,-45 -34,-83 -79,-87l-1 -1c-2,0 -4,0 -6,0 1,0 1,1 1,1l-1 0 1 0c0,2 0,3 0,5l-3 2c-24,23 -48,23 -72,0l-3 -2c0,-2 0,-4 1,-6 -2,0 -4,0 -6,0l-1 1c-45,4 -79,42 -79,87l0 13 74 0 19 0 62 0 19 0 74 0z"/>
      <path fill="#000000" fill-opacity="0.5" d="M90 280l-20 -45c3,-4 5,-7 7,-10 -2,-3 -4,-7 -7,-10l26 -36c2,0 4,0 6,0 -5,35 0,74 7,101l-19 0z"/>
      <path fill="#000000" fill-opacity="0.5" d="M190 280l20 -45c-3,-4 -5,-7 -7,-10 2,-3 4,-7 7,-10l-26 -36c-2,0 -4,0 -6,0 5,35 0,74 -7,101l19 0z"/>
      <path fill="#ffffff" d="M204 250c10,-10 12,-13 23,-2 -8,1 -15,2 -23,2z"/>
      <path fill="#000000" fill-opacity="0.7" d="M180 191c-27,24 -54,23 -80,-1 0,-1 1,-3 1,-5l3 2c24,23 48,23 72,0l3 -2c0,2 1,4 1,6z"/>
      <path fill="#000000" fill-opacity="0.3" d="M109 280l62 0c6,-24 11,-57 9,-89 -2,1 -4,3 -6,5 -4,2 -7,5 -11,7 -21,11 -42,6 -63,-12 -2,32 3,65 9,89z"/>
     </g>
    </svg>
  </div>

  <div @click="showSweater()">
    <svg viewBox="0 0 280 280">
     <g id="c_sweater">
      <path class="tinted" fill="#545454" d="M264 280l0 -15c0,-44 -34,-81 -78,-85l-15 0 0 11c0,3 -1,6 -3,7l0 0c-5,11 -15,19 -28,19 -12,0 -23,-8 -27,-18l-1 -1c-2,-1 -2,-4 -2,-7l0 -11 -16 0c-44,4 -78,41 -78,85l0 15 248 0z"/>
      <path fill="#ffffff" d="M110 191l0 -18c-4,0 -14,9 -14,23 0,10 7,18 16,23 1,-4 7,-7 10,-7 4,0 4,1 5,1l-15 -15c-2,-1 -2,-4 -2,-7z"/>
      <path fill="#ffffff" d="M171 191l0 -18c4,0 13,9 13,23 0,10 -6,18 -16,23 -1,-4 -7,-7 -10,-7 -3,0 -3,1 -5,1l15 -15c2,-1 3,-4 3,-7z"/>
     </g>
    </svg>
  </div>

  <div @click="showVneck()">
    <svg viewBox="0 0 280 280">
     <g id="c_vneck">
      <path class="tinted" fill="#545454" d="M264 290l0 -15c0,-44 -34,-81 -78,-85l-46 47 -46 -47c-44,4 -78,41 -78,85l0 15 248 0z"/>
     </g>
    </svg>
  </div>

  <div @click="showOverall()">
    <svg viewBox="0 0 280 280">
     <g id="c_overall">
      <path fill="#e0e0e0" d="M264 285l0 -15c0,-44 -34,-80 -77,-85 -2,24 -22,43 -46,43 -25,0 -45,-19 -47,-43l0 0c-44,4 -78,41 -78,85l0 15 248 0z"/>
      <path class="tinted" fill="#545454" d="M220 190c-10,-5 -21,-9 -32,-10l0 57 -96 0 0 -57c-11,2 -22,5 -32,11l0 89 160 0 0 -90z"/>
      <circle fill="#000000" fill-opacity="0.5" cx="78" cy="250" r="8"/>
      <circle fill="#000000" fill-opacity="0.5" cx="202" cy="250" r="8"/>
     </g>
    </svg>
  </div>

  <div @click="showHoodie()">
    <svg viewBox="0 0 280 280">
     <g id="c_hoodie">
      <path class="tinted" fill="#545454" d="M264 280l0 -15c0,-36 -24,-68 -56,-80 -1,-13 -17,-20 -39,-23l0 22c0,16 -13,29 -30,29l0 0c-16,0 -29,-13 -29,-29l0 -22c-22,3 -38,10 -39,23 -32,13 -55,44 -55,80l0 15 248 0z"/>
      <path fill="#ffffff" d="M103 212l0 49c0,2 -2,4 -5,4 -2,0 -4,-2 -4,-4l0 -54c2,2 5,3 9,5z"/>
      <path fill="#ffffff" d="M186 217l0 40c0,2 -2,4 -5,4 -2,0 -4,-2 -4,-4l0 -35c3,-2 6,-3 9,-5z"/>
      <path fill="#000000" fill-opacity="0.4" d="M81 175c-4,2 -9,4 -14,7 10,22 36,33 69,37l0 0c-31,-5 -55,-25 -55,-42 0,-1 0,-1 0,-2z"/>
      <path fill="#000000" fill-opacity="0.4" d="M222 192c-4,-3 -9,-5 -14,-7 0,0 0,1 0,2 0,17 -24,37 -55,42l0 0c33,-4 59,-15 69,-37z"/>
     </g>
    </svg>
  </div>

</div>

</template>

<script>
export default {
  name: "OptionsClothes",
  methods: {
    deleteClass() {
      let c = document.getElementById('clothes').children, i;
      for (i = 0; i < c.length; i++) {
        c[i].classList.remove('show');
      }
    },
     showBlazer() {
      this.deleteClass();
      document.querySelector('#c_blazer').classList.add('show');
    },
    showSweater() {
      this.deleteClass();
      document.querySelector('#c_sweater').classList.add('show');
    },
    showVneck() {
      this.deleteClass();
      document.querySelector('#c_vneck').classList.add('show');
    },
    showOverall() {
      this.deleteClass();
      document.querySelector('#c_overall').classList.add('show');
    },
    showHoodie() {
      this.deleteClass();
      document.querySelector('#c_hoodie').classList.add('show');
    }
  }
}
</script>