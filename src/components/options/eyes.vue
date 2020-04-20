<template>
  
<div class="mn">

  <div @click="showDefault()">
    <svg viewBox="0 0 180 180">
     <g id="e_default">
      <circle fill="#000000" fill-opacity="0.7" cx="58" cy="103" r="8"/>
      <circle fill="#000000" fill-opacity="0.7" cx="122" cy="103" r="8"/>
     </g>
    </svg>
  </div>

  <div @click="showDizzy()">
    <svg viewBox="0 0 150 150">
     <g id="e_dizzy">
      <polygon fill="#000000" fill-opacity="0.7" stroke="#5F4A37" stroke-width="0.9" points="89, 91, 96, 99 104, 91 107, 95 100, 102 107, 110 104, 113 96, 106 89, 113 85, 110 93, 102 85, 95"/>
      <polygon fill="#000000" fill-opacity="0.7" stroke="#5F4A37" stroke-width="0.9" points="39, 91, 46, 99 54, 91 57, 95 50, 102 57, 110 54, 113 46, 106 39, 113 35, 110 43, 102 35, 95"/>
     </g>
    </svg>
  </div>

  <div @click="showEyeroll()">
    <svg viewBox="0 0 150 150">
     <g id="e_eyeroll">
      <circle fill="#cecece" cx="43" cy="112" r="17"/>
      <circle fill="#4D4D4D" stroke="#5F4A37" stroke-width="0.9" cx="43" cy="103" r="8"/>
      <circle fill="#cecece" cx="117" cy="112" r="17"/>
      <circle fill="#4D4D4D" cx="117" cy="103" r="8"/>
     </g>
    </svg>
  </div>

  <div @click="showHappy()">
    <svg viewBox="0 0 150 150">
     <g id="e_happy">
      <path fill="#000000" fill-opacity="0.7" d="M31 100c-1,0 0,2 1,1 2,-2 5,-3 11,-4 7,1 9,2 11,4 2,1 3,-1 2,-1 -1,-1 -5,-7 -13,-7 -7,0 -12,6 -12,7z"/>
      <path fill="#000000" fill-opacity="0.7" d="M102 100c0,0 1,2 2,1 2,-2 5,-3 11,-4 7,1 9,2 11,4 2,1 3,-1 2,-1 -1,-1 -5,-7 -13,-7 -7,0 -12,6 -13,7z"/>
     </g>
    </svg>
  </div>

  <div @click="showClose()">
    <svg viewBox="0 0 150 150">
     <g id="e_close">
      <path fill="#000000" fill-opacity="0.7" d="M31 100c-1,0 0,-2 1,-1 2,2 5,3 11,4 7,-1 9,-2 11,-4 2,-1 3,1 2,1 -1,1 -5,7 -13,7 -7,0 -12,-6 -12,-7z"/>
      <path fill="#000000" fill-opacity="0.7" d="M102 100c0,0 1,-2 2,-1 2,2 5,3 11,4 7,-1 9,-2 11,-4 2,-1 3,1 2,1 -1,1 -5,7 -13,7 -7,0 -12,-6 -13,-7z"/>
     </g>
    </svg>
  </div>

  <div @click="showHearts()">
    <svg viewBox="0 0 150 150">
     <g id="e_hearts">
      <path fill="#FC675E" d="M30 80c4,0 7,2 9,5 1,-3 5,-5 8,-5 6,0 10,4 10,10 0,2 -1,5 -3,7 -5,5 -10,10 -15,16l-16 -16c-2,-2 -3,-5 -3,-7 0,-6 4,-10 10,-10z"/>
      <path fill="#FC675E" d="M100 80c4,0 7,2 9,5 2,-3 5,-5 9,-5 5,0 10,4 10,10 0,2 -2,5 -3,7 -5,5 -11,10 -16,16l-16 -16c-2,-2 -3,-5 -3,-7 0,-6 5,-10 10,-10z"/>
     </g>
    </svg>
  </div>

  <div @click="showSide()">
    <svg viewBox="0 0 150 150">
     <g id="e_side">
      <path fill="#000000" fill-opacity="0.7" d="M129 95c0,4 -3,7 -7,7 -5,0 -8,-3 -8,-7 0,-2 1,-3 1,-5 -6,1 -9,2 -11,4 -2,1 -2,-1 -2,-1 1,-1 6,-8 14,-8 4,0 8,2 10,4 2,1 3,3 3,6z"/>
      <path fill="#000000" fill-opacity="0.7" d="M57 95c0,4 -3,7 -7,7 -4,0 -8,-3 -8,-7 0,-2 1,-3 2,-5 -7,1 -10,2 -12,4 -1,1 -2,-1 -1,-1 0,-1 6,-8 13,-8 4,0 8,2 11,4 1,1 2,3 2,6z"/>
     </g>
    </svg>
  </div>

  <div @click="showWink()">
    <svg viewBox="0 0 150 150">
     <g id="e_wink">
      <path fill="#000000" fill-opacity="0.7" d="M125 95c1,1 0,3 -2,1 -2,-1 -4,-3 -11,-3 -6,0 -9,2 -11,3 -1,2 -2,0 -2,-1 1,-1 6,-7 13,-7 8,0 12,6 13,7z"/>
      <circle fill="#000000" fill-opacity="0.7" cx="48" cy="93" r="7"/>
     </g>
    </svg>
  </div>

  <div @click="showSquint()">
    <svg viewBox="0 0 150 150">
     <g id="e_squint">
      <path fill="#cecece" d="M45 100c-6,0 -13,1 -17,1 0,-1 0,-2 0,-3 0,-9 7,-16 17,-16 9,0 16,7 16,16 0,1 0,2 0,3 -3,0 -11,-1 -16,-1z"/>
      <path fill="#4D4D4D" d="M45 100c-2,0 -3,0 -4,0 -2,-1 -4,-3 -4,-6 0,-3 3,-6 8,-6 4,0 7,3 7,6 0,3 -1,5 -3,6 -2,0 -3,0 -4,0z"/>
      <path fill="#cecece" d="M109 100c-5,0 -13,1 -16,1 0,-1 0,-2 0,-3 0,-9 7,-16 16,-16 10,0 17,7 17,16 0,1 0,2 0,3 -4,0 -11,-1 -17,-1z"/>
      <path fill="#4D4D4D" d="M109 100c-1,0 -2,0 -4,0 -2,-1 -3,-3 -3,-6 0,-3 3,-6 7,-6 4,0 8,3 8,6 0,3 -2,5 -4,6 -1,0 -2,0 -4,0z"/>
     </g>
    </svg>
  </div>

  <div @click="showSurprised()">
    <svg viewBox="0 0 150 150">
     <g id="e_surprised">
      <circle fill="#FEFEFE" cx="48" cy="100" r="17"/>
      <circle fill="#4D4D4D" stroke="#5F4A37" stroke-width="0.9" cx="48" cy="100" r="8"/>
      <circle fill="#FEFEFE" cx="112" cy="100" r="17"/>
      <circle fill="#4D4D4D" cx="112" cy="100" r="8"/>
     </g>
    </svg>
  </div>

  <div @click="showWinkwacky()">
    <svg viewBox="0 0 150 150">
     <g id="e_winkwacky">
      <path fill="#000000" fill-opacity="0.7" d="M31 106c-1,1 0,3 1,1 2,-1 5,-3 11,-3 7,0 9,2 11,3 2,2 3,0 2,-1 -1,-1 -5,-7 -13,-7 -7,0 -12,6 -12,7z"/>
      <circle fill="#FEFEFE" cx="112" cy="103" r="15"/>
      <circle fill="#4D4D4D" cx="112" cy="103" r="8"/>
     </g>
    </svg>
  </div>

  <div @click="showCry()">
    <svg viewBox="0 0 150 150">
     <g id="e_cry">
      <circle fill="#000000" fill-opacity="0.7" cx="48" cy="103" r="8"/>
      <circle fill="#000000" fill-opacity="0.7" cx="102" cy="103" r="8"/>
      <path fill="#92D9FF" d="M44 123c0,-3 6,-12 8,-14 2,2 7,11 7,14 0,4 -3,8 -7,8 0,0 0,0 0,0 0,0 0,0 0,0 -4,0 -8,-4 -8,-8z"/>
     </g>
    </svg>
  </div>

</div>

</template>

<script>
export default {
  name: "OptionsEyes",
  methods: {
    deleteClass() {
      let c = document.getElementById('eyes').children, i;
      for (i = 0; i < c.length; i++) {
        c[i].classList.remove('show');
      }
    },
    showDefault() {
      this.deleteClass();
      document.querySelector('#e_default').classList.add('show');
    },
    showDizzy() {
      this.deleteClass();
      document.querySelector('#e_dizzy').classList.add('show');
    },
    showEyeroll() {
      this.deleteClass();
      document.querySelector('#e_eyeroll').classList.add('show');
    },
    showHappy(){
      this.deleteClass();
      document.querySelector('#e_happy').classList.add('show');
    },
    showClose() {
      this.deleteClass();
      document.querySelector('#e_close').classList.add('show');
    },
    showHearts() {
      this.deleteClass();
      document.querySelector('#e_hearts').classList.add('show');
    },
    showSide() {
      this.deleteClass();
      document.querySelector('#e_side').classList.add('show');
    },
    showWink() {
      this.deleteClass();
      document.querySelector('#e_wink').classList.add('show');
    },
    showSquint() {
      this.deleteClass();
      document.querySelector('#e_squint').classList.add('show');
    },
    showSurprised() {
      this.deleteClass();
      document.querySelector('#e_surprised').classList.add('show');
    },
    showWinkwacky() {
      this.deleteClass();
      document.querySelector('#e_winkwacky').classList.add('show');
    },
    showCry() {
      this.deleteClass();
      document.querySelector('#e_cry').classList.add('show');
    }
  }
}
</script>