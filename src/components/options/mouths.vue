<template>

<div class="mn">

  <div @click="showVomit()">
    <svg viewBox="0 0 100 100">
     <g id="m_vomit">
      <path fill="#000000" d="M50 33l0 0c13,0 24,11 24,25l0 2 -48 0 0 -2c0,-14 11,-25 24,-25z"/>
      <path fill="#FEFEFE" d="M50 33l0 0c6,0 12,3 17,7l-34 0c5,-4 11,-7 17,-7z"/>
      <path fill="#88C553" d="M35 51l30 0c4,0 8,4 8,8l0 6c0,4 -4,7 -8,7 -4,0 -7,-3 -7,-7 0,-3 -4,-5 -8,-5 -4,0 -7,4 -7,8 0,5 -4,8 -8,8 -4,0 -7,-3 -7,-8l0 -9c0,-4 3,-8 7,-8z"/>
     </g>
    </svg>
  </div>

  <div @click="showTwinkle()">
    <svg viewBox="0 0 100 100">
     <g id="m_twinkle">
      <path fill="#000000" fill-rule="nonzero" d="M32 50c-1,-2 0,-3 2,-3 1,-1 3,0 3,1 1,3 2,5 5,6 2,2 5,3 8,3 3,0 6,-1 8,-3 3,-1 4,-3 5,-6 0,-1 2,-2 3,-1 2,0 3,1 2,3 -1,3 -4,6 -7,9 -3,2 -7,3 -11,3 -4,0 -8,-1 -11,-3 -3,-3 -6,-6 -7,-9z"/>
     </g>
    </svg>
  </div>

  <div @click="showTongue()">
    <svg viewBox="0 0 100 100">
     <g id="m_tongue">
      <path fill="#000000" d="M50 70l0 0c17,0 31,-10 31,-23l0 -1 -62 0 0 1c0,13 14,23 31,23z"/>
      <path fill="#FEFEFE" d="M69 46l-38 0 0 2c0,3 2,5 4,5l30 0c2,0 4,-2 4,-5l0 -2z"/>
      <path fill="#FF4F6D" d="M64 70l0 0c0,8 -6,15 -14,15l0 0c-8,0 -14,-7 -14,-15l0 0 0 -7c0,-4 4,-8 8,-8 3,0 5,1 6,2 1,-1 3,-2 6,-2 4,0 8,4 8,8l0 7z"/>
     </g>
    </svg>
  </div>

  <div @click="showSmile()">
    <svg viewBox="0 0 100 100">
     <g id="m_smile">
      <path fill="#000000" d="M50 70l0 0c13,0 24,-10 24,-23l0 -1 -48 0 0 1c0,13 11,23 24,23z"/>
      <path fill="#FF4F6D" d="M50 70l0 0c6,0 11,-2 16,-5 -2,-3 -5,-5 -9,-5 -3,0 -5,1 -7,2 -2,-1 -4,-2 -7,-2 -4,0 -7,2 -9,5 5,3 10,5 16,5z"/>
      <path fill="#FEFEFE" d="M69 46l-38 0 0 2c0,3 2,5 4,5l30 0c2,0 4,-2 4,-5l0 -2z"/>
     </g>
    </svg>
  </div>

  <div @click="showSerious()">
    <svg viewBox="0 0 100 100">
     <g id="m_serious">
      <path fill="#000000" d="M38 53l24 0c2,0 3,2 3,4l0 0c0,2 -1,3 -3,3l-24 0c-2,0 -3,-1 -3,-3l0 0c0,-2 1,-4 3,-4z"/>
     </g>
    </svg>
  </div>

  <div @click="showScream()">
    <svg viewBox="0 0 100 100">
     <g id="m_scream">
      <path fill="#000000" d="M50 36l0 0c14,0 24,11 24,24 0,4 0,8 0,11 -8,-1 -16,-2 -24,-2 -8,0 -16,1 -24,2l0 -11c0,-13 10,-24 24,-24z"/>
      <path fill="#e8e8e8" d="M50 37l0 0c7,0 13,2 17,7l-34 0c4,-5 10,-7 17,-7z"/>
      <path fill="#FF4F6D" d="M50 62c-2,-2 -4,-2 -6,-2 -3,0 -8,1 -9,4 -2,2 -3,3 -5,7 7,-1 13,-2 20,-2l0 0 0 0c7,0 13,1 20,2 -2,-4 -3,-5 -5,-7 -1,-3 -6,-4 -9,-4 -2,0 -4,0 -6,2z"/>
     </g>
    </svg>
  </div>

  <div @click="showGrimace()">
    <svg viewBox="0 0 120 120">
     <g id="m_grimace">
      <path fill="#FEFEFE" fill-rule="nonzero" d="M84 62l-48 0c-3,0 -7,1 -9,4 -3,2 -4,5 -4,9 0,4 1,7 4,9 2,3 6,4 9,4l48 0c3,0 7,-1 9,-4 3,-2 4,-5 4,-9 0,-4 -1,-7 -4,-9 -2,-3 -6,-4 -9,-4z"/>
      <path fill="#B2B3B3" d="M23 64l11 0 0 -12c1,0 2,0 2,0l2 0 0 12 12 0 0 -12 4 0 0 12 12 0 0 -12 4 0 0 12 12 0 0 -12 2 0c0,0 1,0 2,0l0 12 11 0c0,0 0,1 0,1 0,1 0,1 0,2l-11 0 0 11c-1,0 -2,0 -2,0l-2 0 0 -11 -12 0 0 11 -4 0 0 -11 -12 0 0 11 -4 0 0 -11 -12 0 0 11 -2 0c0,0 -1,0 -2,0l0 -11 -11 0c0,-1 0,-1 0,-2 0,0 0,-1 0,-1z"/>
      <path fill="#000000" fill-rule="nonzero" d="M36 48l48 0c4,0 9,2 12,5 3,3 5,8 5,12 0,5 -2,9 -5,12 -3,3 -8,5 -12,5l-48 0c-4,0 -9,-2 -12,-5 -3,-3 -5,-7 -5,-12 0,-4 2,-9 5,-12 3,-3 8,-5 12,-5zm48 4l-48 0c-3,0 -7,1 -9,4 -3,2 -4,5 -4,9 0,4 1,7 4,9 2,3 6,4 9,4l48 0c3,0 7,-1 9,-4 3,-2 4,-5 4,-9 0,-4 -1,-7 -4,-9 -2,-3 -6,-4 -9,-4z"/>
     </g>
    </svg>
  </div>

  <div @click="showEating()">
    <svg viewBox="0 0 100 100">
     <g id="m_eating">
      <circle fill="#E08C65" fill-opacity="0.6" cx="15" cy="59" r="11"/>
      <circle fill="#E08C65" fill-opacity="0.6" cx="85" cy="59" r="11"/>
      <path fill="#000000" d="M38 61c9,3 18,3 26,0 0,-6 5,-12 12,-13 -5,3 -8,7 -8,12 0,8 7,14 14,14 1,0 1,0 1,0 -2,1 -3,1 -5,1 -7,0 -12,-4 -14,-9 -9,3 -18,3 -27,0 -2,5 -7,8 -13,8 -2,0 -3,0 -5,-1 0,0 0,0 1,0 7,0 14,-6 14,-14 0,-5 -3,-10 -8,-12 7,1 12,7 12,14 0,0 0,0 0,0z"/>
     </g>
    </svg>
  </div>

  <div @click="showDisbelief()">
    <svg viewBox="0 0 80 80">
     <g id="m_disbelief">
      <path fill="#000000" d="M40 39l0 0c10,0 17,8 17,17l0 1 -34 0 0 -1c0,-9 7,-17 17,-17z"/>
     </g>
    </svg>
  </div>

  <div @click="showDefault()">
    <svg viewBox="0 0 80 80">
     <g id="m_default">
      <path fill="#000000" d="M40 60l0 0c10,0 17,-8 17,-18l0 0 -34 0 0 0c0,10 7,18 17,18z"/>
     </g>
    </svg>
  </div>

  <div @click="showConcerned()">
    <svg viewBox="0 0 80 80">
     <g id="m_concerned">
      <path fill="#000000" d="M40 37l0 0c13,0 24,10 24,23l0 1 -48 0 0 -1c0,-13 11,-23 24,-23z"/>
      <path fill="#FEFEFE" d="M40 38l0 0c6,0 12,2 16,6l-32 0c4,-4 10,-6 16,-6z"/>
      <path fill="#FF4F6D" d="M33 51c4,0 5,1 7,3 2,-2 3,-3 7,-3 5,0 11,5 12,10l-38 0c1,-5 7,-10 12,-10z"/>
     </g>
    </svg>
  </div>


</div>

</template>


<script>
export default {
  name: "OptionsMouths",
  methods: {
    deleteClass() {
      let c = document.getElementById('mouths').children, i;
      for (i = 0; i < c.length; i++) {
        c[i].classList.remove('show');
      }
    },
    showVomit() {
      this.deleteClass();
      document.querySelector('#m_vomit').classList.add('show');
    },
    showTwinkle() {
      this.deleteClass();
      document.querySelector('#m_twinkle').classList.add('show');
    },
    showTongue() {
      this.deleteClass();
      document.querySelector('#m_tongue').classList.add('show');
    },
    showSmile() {
      this.deleteClass();
      document.querySelector('#m_smile').classList.add('show');
    },
    showSerious() {
      this.deleteClass();
      document.querySelector('#m_serious').classList.add('show');
    },
    showScream() {
      this.deleteClass();
      document.querySelector('#m_scream').classList.add('show');
    },
    showGrimace() {
      this.deleteClass();
      document.querySelector('#m_grimace').classList.add('show');
    },
    showEating() {
      this.deleteClass();
      document.querySelector('#m_eating').classList.add('show');
    },
    showDisbelief() {
      this.deleteClass();
      document.querySelector('#m_disbelief').classList.add('show');
    },
    showDefault() {
      this.deleteClass();
      document.querySelector('#m_default').classList.add('show');
    },
    showConcerned() {
      this.deleteClass();
      document.querySelector('#m_concerned').classList.add('show');
    }
  }
}
</script>