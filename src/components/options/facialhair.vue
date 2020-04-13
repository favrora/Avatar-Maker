<template>

<div class="mn">

  <div @click="showMagestic()">
    <svg viewBox="0 0 200 200">
     <g id="f_magestic">
      <path class="tinted" fill="#6f2912" d="M30 30c1,11 -1,61 16,60 9,0 20,-15 29,-16 13,-1 20,0 24,5 4,-5 11,-6 24,-5 9,1 20,16 29,16 17,1 15,-49 16,-60 2,13 5,25 5,38 1,11 -2,22 -4,34 -1,11 0,24 -4,35 -2,7 -9,12 -13,18 -3,3 -5,8 -8,10 -5,3 -11,3 -16,6 -18,7 -10,8 -29,8 -19,0 -11,-1 -29,-8 -5,-3 -11,-3 -16,-6 -3,-2 -5,-7 -8,-10 -4,-6 -11,-11 -13,-18 -4,-11 -3,-24 -4,-35 -2,-12 -5,-23 -4,-34 0,-13 3,-25 5,-38zm69 56c-3,3 -7,4 -13,5 -6,2 -15,4 -15,14 0,7 7,14 13,15 8,1 5,-4 15,-4 10,0 7,5 15,4 6,-1 13,-8 13,-15 0,-10 -9,-12 -15,-14 -6,-1 -10,-2 -13,-5z"/>
     </g>
    </svg>
  </div>

  <div @click="showMagnum()">
    <svg viewBox="0 0 100 100">
      <g id="f_magnum">
      <path class="tinted" fill="#6f2912" d="M40 70c7,-1 10,-4 10,-10 0,6 3,9 10,10 10,1 12,-3 20,-3 7,1 8,2 10,2 1,0 1,-1 1,-2 -6,-16 -26,-17 -31,-16 -6,1 -10,4 -10,9 0,-5 -4,-8 -10,-9 -5,-1 -25,0 -31,16 0,1 0,2 1,2 2,0 3,-1 10,-2 8,0 10,4 20,3z"/>
    </g>
    </svg>
  </div>

  <div @click="showFancy()">
    <svg viewBox="0 0 120 120">
      <g id="f_fancy">
      <path class="tinted" fill="#6f2912" d="M7 70c2,2 18,0 24,-5 6,-5 20,-5 25,-1 2,2 1,5 0,5 -7,4 -15,7 -22,9 -12,4 -21,1 -27,-7 -1,-1 0,-2 0,-1zm106 0c-2,2 -18,0 -24,-5 -6,-5 -20,-5 -25,-1 -2,2 -1,5 0,5 7,4 15,7 22,9 12,4 21,1 27,-7 1,-1 0,-2 0,-1z"/>
    </g>
    </svg>
  </div>

  <div @click="showLight()">
    <svg viewBox="0 0 200 200">
      <g id="f_light">
      <path class="tinted" fill="#6f2912" d="M90 100c-5,0 -7,0 -12,0 -6,0 -12,7 -15,13 -3,4 -4,10 -10,8 -14,-2 -20,-19 -20,-36l0 -27c0,-4 -3,-6 -6,-6 0,15 0,30 0,45 0,41 31,66 69,66 38,0 69,-25 69,-66 0,-15 0,-30 0,-45 -3,0 -6,2 -6,6l0 27c0,17 -6,34 -20,36 -6,2 -7,-4 -10,-8 -3,-6 -9,-13 -15,-13 -5,0 -7,0 -12,0 -3,0 -6,2 -6,5 0,3 3,6 6,6 5,0 8,-1 14,0 7,0 10,9 9,14 0,6 -3,12 -6,16 -3,3 -7,5 -11,5 -5,0 -5,-6 -12,-6 -7,0 -7,6 -12,6 -4,0 -8,-2 -11,-5 -3,-4 -6,-10 -6,-16 -1,-5 2,-14 9,-14 6,-1 9,0 14,0 3,0 6,-3 6,-6 0,-3 -3,-5 -6,-5z"/>
    </g>
    </svg>
  </div>

</div>

</template>


<script>
export default {
  name: "OptionsFacialHair",
  methods: {
    deleteClass() {
      let c = document.getElementById('facialhair2').children, i;
      for (i = 0; i < c.length; i++) {
        c[i].classList.remove('show');
      }
    },
    showMagestic() {
      if(document.querySelector('#f_magestic').classList.contains('show')) {
        this.deleteClass();
      } else {
        this.deleteClass();
        document.querySelector('#f_magestic').classList.add('show');
      }
    },
    showMagnum() {
      if(document.querySelector('#f_magnum').classList.contains('show')) {
        this.deleteClass();
      } else {
        this.deleteClass();
        document.querySelector('#f_magnum').classList.add('show');
      }
    },
    showFancy() {
      if(document.querySelector('#f_fancy').classList.contains('show')) {
        this.deleteClass();
      } else {
        this.deleteClass();
        document.querySelector('#f_fancy').classList.add('show');
      }
    },
    showLight() {
      if(document.querySelector('#f_light').classList.contains('show')) {
        this.deleteClass();
      } else {
        this.deleteClass();
        document.querySelector('#f_light').classList.add('show');
      }
    }
  }
}
</script>