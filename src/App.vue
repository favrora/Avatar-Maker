<template>
  <div id="app">
    <div id="avatar">
      <OptionsColor />
      <Github />
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

// import options color
import OptionsColor from './components/optionsColor'

// import footer
import Footer from './components/footer'

// Github icon component
import Github from './components/layout/githubIcon'

export default {
  name: 'App',
  metaInfo: {
    title: 'Avatar Maker - Create your own avatar online',
    htmlAttrs: {
      lang: 'en'
    },

    meta: [
      // Meta Seo
      { vmid: 'robots', name: 'robots', content: 'index, follow' },
      { vmid: 'description', name: 'description', content: 'Collect your avatar from different parts. Create your own avatar with Avatar Maker and download avatar image. Avatar Maker is absolutely free.' },
      { vmid: 'theme-color', name: 'theme-color', content: '#0077FF' },

      // Open Graph
      { vmid: 'og:locale', property: 'og:locale', content: 'en_US' },
      { vmid: 'og:site_name', property: 'og:site_name', content: 'Avatar Maker' },
      { vmid: 'og:type', property: 'og:type', content: 'website' },
      { vmid: 'og:image', property: 'og:image', content: 'https://github.com/favrora/Avatar-Maker/blob/master/src/assets/img/preview.jpg' },

      // Twitter
      { vmid: 'twitter:card', property: 'twitter:card', content: 'summary_large_image' },
      { vmid: 'twitter:creator', property: 'twitter:creator', content: 'favrora_com' },
    ],
  },

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
    OptionsColor,
    Github
  },

  methods: {
    resetAvatar() {
      this.$root.$refs.Accesories.picker('#g_none');
      this.$root.$refs.Clothes.picker('#c_none');
      this.$root.$refs.Eyebrows.picker('#eb_none');
      this.$root.$refs.Eyes.picker('#e_none');
      this.$root.$refs.FacialHair.picker('#f_none');
      this.$root.$refs.Glasses.picker('#g_none');
      this.$root.$refs.Hair.picker('#h_none');
      this.$root.$refs.Mouths.picker('#m_none');
      this.$root.$refs.SkinColor.picker('#skin_white');
      this.$root.$refs.Tattoos.picker('#t_none');
    },
    randomAvatar() {
      this.$root.$refs.Accesories.picker();
      this.$root.$refs.Clothes.picker();
      this.$root.$refs.Eyebrows.picker();
      this.$root.$refs.Eyes.picker();
      this.$root.$refs.FacialHair.picker();
      this.$root.$refs.Glasses.picker();
      this.$root.$refs.Hair.picker();
      this.$root.$refs.Mouths.picker();
      this.$root.$refs.SkinColor.picker();
      this.$root.$refs.Tattoos.picker();
    }
  },

  mounted() {
    window.addEventListener('load', () => {
      this.randomAvatar();
    })
  },

  created() {
    this.$root.$refs.App = this;
  }
}
</script>

// import scss
<style lang="scss">
@import "./assets/sass/variables";
@import "./assets/sass/responsive";
@import "./assets/sass/avatar";
@import "./assets/sass/footer";
@import "./assets/sass/save_image";
@import "./assets/sass/options_color";
</style>