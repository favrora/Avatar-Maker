<template>
  <div id="app">
    <div id="avatar">
      <Accesories />
      <Clothes />
      <Eyebrows />
      <Eyes />
      <Facialhair />
      <Glasses />
      <Hair />
      <Mounths />
      <SkinColor />
      <Tattoos />
    </div>
    <Footer />
    <SaveImage/>
  </div>
</template>

<script>
// import avatar component
import Accesories  from './components/layout/accesories'
import Clothes     from './components/layout/clothes'
import Eyebrows    from './components/layout/eyebrows'
import Eyes        from './components/layout/eyes'
import Facialhair  from './components/layout/facialhair'
import Glasses     from './components/layout/glasses'
import Hair        from './components/layout/hair'
import Mounths     from './components/layout/mouths'
import SkinColor   from './components/layout/SkinColor'
import Tattoos     from './components/layout/tattoos'

// import footer
import Footer      from './components/footer'

// import save Image
import SaveImage   from './components/save_image'

export default {
  name: 'App',
  components: {
    Accesories,
    Clothes,
    Eyebrows,
    Eyes,
    Facialhair,
    Glasses,
    Hair,
    Mounths,
    SkinColor,
    Tattoos,
    Footer,
    SaveImage
  }
}
</script>

// import scss
<style lang="scss">
@import "./assets/sass/variables";
@import "./assets/sass/responsive";
@import "./assets/sass/avatar";
@import "./assets/sass/footer";
@import "./assets/sass/save_image"
</style>
