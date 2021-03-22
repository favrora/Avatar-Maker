<template>
  
<div class="mn">

  <div @click="showDefault()">
    <svg viewBox="0 0 150 150">
     <g id="eb_default">
      <path fill="#000000" fill-opacity="0.7" fill-rule="nonzero" d="M25 100c-1,1 -3,1 -4,0 -1,-1 -1,-2 0,-3 5,-6 10,-9 16,-11 6,-2 13,-2 20,0 2,0 3,2 2,3 0,2 -1,3 -3,2 -6,-1 -12,-2 -17,0 -5,1 -10,4 -14,9z"/>
      <path fill="#000000" fill-opacity="0.7" fill-rule="nonzero" d="M129 100c1,1 2,1 3,0 2,-1 2,-2 1,-3 -5,-6 -11,-9 -17,-11 -6,-2 -13,-2 -20,0 -1,0 -2,2 -2,3 1,2 2,3 3,2 7,-1 13,-2 18,0 5,1 10,4 14,9z"/>
     </g>
    </svg>
  </div>

  <div @click="showDefault2()">
    <svg viewBox="0 0 150 150">
     <g id="eb_default2">
      <path fill="#000000" fill-opacity="0.7" d="M20 100c5,-4 11,-5 18,-6 5,-1 12,-1 20,1 -5,-6 -14,-10 -22,-7 -7,1 -13,5 -16,12z"/>
      <path fill="#000000" fill-opacity="0.7" d="M133 100c-5,-4 -12,-5 -18,-6 -5,-1 -12,-1 -20,1 5,-6 14,-10 22,-7 7,1 13,5 16,12z"/>
     </g>
    </svg>
  </div>

  <div @click="showRaised()">
    <svg viewBox="0 0 150 150">
     <g id="eb_raised">
      <path fill="#000000" fill-opacity="0.7" d="M20 100c5,-4 8,-10 14,-13 7,-3 12,-5 23,-5 -10,-3 -20,-4 -27,0 -6,4 -9,11 -10,18z"/>
      <path fill="#000000" fill-opacity="0.7" d="M129 100c-5,-4 -8,-10 -14,-13 -8,-3 -12,-5 -23,-5 10,-3 20,-4 26,0 6,4 10,11 11,18z"/>
     </g>
    </svg>
  </div>

  <div @click="showSad()">
    <svg viewBox="0 0 150 150">
     <g id="eb_sad">
      <path fill="#000000" fill-opacity="0.7" fill-rule="nonzero" d="M20 100c-2,-1 -2,-2 -2,-4 1,-1 3,-2 4,-1 0,0 1,0 1,1 6,2 12,2 17,0 5,-2 9,-6 12,-13 0,0 0,-1 1,-1 0,-2 2,-2 3,-2 2,1 2,2 2,4 -1,0 -1,1 -1,2 -4,7 -9,12 -15,15 -6,3 -14,3 -21,0 0,-1 -1,-1 -1,-1z"/>
      <path fill="#000000" fill-opacity="0.7" fill-rule="nonzero" d="M129 100c2,-1 2,-2 1,-4 0,-1 -2,-2 -3,-1 -1,0 -1,0 -1,1 -6,2 -12,2 -17,0 -5,-2 -9,-6 -12,-13 0,0 -1,-1 -1,-1 -1,-2 -2,-2 -3,-2 -2,1 -2,2 -2,4 0,0 1,1 1,2 4,7 9,12 15,15 6,3 13,3 21,0 0,-1 1,-1 1,-1z"/>
     </g>
    </svg>
  </div>

  <div @click="showSad2()">
    <svg viewBox="0 0 150 150">
     <g id="eb_sad2">
      <path fill="#000000" fill-opacity="0.7" d="M20 100c7,0 18,-1 22,-4 5,-4 11,-9 15,-15 0,5 -4,15 -10,19 -7,4 -20,4 -27,0z"/>
      <path fill="#000000" fill-opacity="0.7" d="M130 100c-8,0 -18,-1 -23,-4 -5,-4 -10,-9 -14,-15 0,5 3,15 10,19 7,4 19,4 27,0z"/>
     </g>
    </svg>
  </div>

  <div @click="showUnibrow()">
    <svg viewBox="0 0 150 150">
     <g id="eb_unibrow">
      <path fill="#000000" fill-opacity="0.7" d="M15 100c3,-5 10,-11 17,-12 7,-1 14,3 20,4 7,1 13,3 20,4 -7,4 -12,4 -18,4 -7,0 -15,-4 -22,-4 -6,0 -11,2 -17,4z"/>
      <path fill="#000000" fill-opacity="0.7" d="M135 100c-3,-5 -10,-11 -17,-12 -7,-1 -14,3 -20,4 -7,1 -13,3 -20,4 7,4 12,4 18,4 7,0 15,-4 22,-4 6,0 11,2 17,4z"/>
     </g>
    </svg>
  </div>

  <div @click="showUpdown()">
    <svg viewBox="0 0 150 150">
     <g id="eb_updown">
      <path fill="#000000" fill-opacity="0.7" fill-rule="nonzero" d="M25 104c-1,1 -2,1 -4,0 -1,-1 -1,-3 0,-4 7,-7 13,-10 20,-12 6,-1 12,0 18,3 2,1 2,2 2,4 -1,1 -3,2 -4,1 -5,-3 -10,-4 -15,-2 -6,1 -11,4 -17,10z"/>
      <path fill="#000000" fill-opacity="0.7" fill-rule="nonzero" d="M134 109c1,1 0,3 -1,4 -1,1 -2,1 -3,0 -5,-5 -10,-8 -16,-9 -6,-2 -12,-2 -16,0 -2,1 -3,0 -4,-1 0,-1 0,-3 2,-4 5,-2 13,-2 20,-1 6,2 12,6 18,11z"/>
     </g>
    </svg>
  </div>

  <div @click="showUpdown2()">
    <svg viewBox="0 0 150 150">
     <g id="eb_updown2">
      <path fill="#000000" fill-opacity="0.7" d="M26 106c5,-4 8,-10 14,-13 7,-3 12,-5 23,-5 -10,-3 -20,-4 -27,0 -6,4 -9,11 -10,18z"/>
      <path fill="#000000" fill-opacity="0.7" d="M137 115c-6,-3 -11,-7 -18,-8 -8,-1 -13,-2 -23,2 8,-6 17,-10 25,-8 7,2 12,7 16,14z"/>
     </g>
    </svg>
  </div>

  <div @click="showAngry()">
    <svg viewBox="0 0 150 150">
     <g id="eb_angry">
      <path fill="#000000" fill-opacity="0.7" fill-rule="nonzero" d="M22 100c-2,1 -3,1 -4,-1 -1,-1 -1,-3 1,-3 1,-1 2,-2 3,-3 3,-3 6,-5 10,-5 3,-1 5,0 8,2 2,1 4,3 6,5 2,1 3,3 5,3 1,1 3,1 5,1 1,0 3,0 3,2 0,1 -1,3 -2,3 -3,1 -6,0 -8,-1 -3,-1 -5,-2 -7,-4 -1,-2 -3,-3 -5,-5 -1,-1 -3,-1 -5,-1 -2,0 -4,2 -6,4 -2,1 -3,2 -4,3z"/>
      <path fill="#000000" fill-opacity="0.7" fill-rule="nonzero" d="M128 100c1,1 3,1 4,-1 1,-1 0,-3 -1,-3 -1,-1 -2,-2 -3,-3 -3,-3 -6,-5 -10,-5 -3,-1 -6,0 -8,2 -2,1 -5,3 -6,5 -2,1 -3,3 -5,3 -2,1 -3,1 -5,1 -1,0 -3,0 -3,2 0,1 0,3 2,3 3,1 5,0 8,-1 2,-1 4,-2 6,-4 2,-2 4,-3 6,-5 1,-1 3,-1 5,-1 2,0 4,2 6,4 1,1 3,2 4,3z"/>
     </g>
    </svg>
  </div>

  <div @click="showAngry2()">
    <svg viewBox="0 0 150 150">
     <g id="eb_angry2">
      <path fill="#000000" fill-opacity="0.7" d="M20 100c1,-4 5,-8 10,-7 5,1 9,3 13,6 5,3 12,8 17,9 -5,3 -10,2 -13,0 -5,-2 -10,-7 -16,-9 -3,-1 -7,0 -11,1z"/>
      <path fill="#000000" fill-opacity="0.7" d="M130 100c-1,-4 -5,-8 -10,-7 -5,1 -9,3 -13,6 -5,3 -12,8 -17,9 5,3 9,2 13,0 5,-2 10,-7 15,-9 4,-1 8,0 12,1z"/>
     </g>
    </svg>
  </div>

</div>

</template>


<script>
export default {
  name: "OptionsEyebrows",
  methods: {
    deleteClass() {
      let c = document.getElementById('eyebrows').children, i;
      for (i = 0; i < c.length; i++) {
        c[i].classList.remove('show');
      }
    },
    showDefault() {
      this.deleteClass();
      document.querySelector('#eb_default').classList.add('show');
    },
    showDefault2() {
      this.deleteClass();
      document.querySelector('#eb_default2').classList.add('show');
    },
    showRaised() {
      this.deleteClass();
      document.querySelector('#eb_raised').classList.add('show');
    },
    showSad() {
      this.deleteClass();
      document.querySelector('#eb_sad').classList.add('show');
    },
    showSad2() {
      this.deleteClass();
      document.querySelector('#eb_sad2').classList.add('show');
    },
    showUnibrow() {
      this.deleteClass();
      document.querySelector('#eb_unibrow').classList.add('show');
    },
    showUpdown() {
      this.deleteClass();
      document.querySelector('#eb_updown').classList.add('show');
    },
    showUpdown2() {
      this.deleteClass();
      document.querySelector('#eb_updown2').classList.add('show');
    },
    showAngry() {
      this.deleteClass();
      document.querySelector('#eb_angry').classList.add('show');
    },
    showAngry2() {
      this.deleteClass();
      document.querySelector('#eb_angry2').classList.add('show');
    }
  }
}
</script>