<template>
  <div id="save-image">
    <button type="button" class="save-button" @click="saveImage">Download Avatar</button>
  </div>
</template>

<script>
import Canvg from 'canvg';

export default {
  name: 'SaveImage',
  methods: {
    async saveImage() {
      const avatarDiv = document.querySelector('#avatar');

      let combinedSvg = '<svg width="100%" height="100%">';

      function addIfAvailable(element) {
        if (element !== undefined && element !== null) {
          combinedSvg = combinedSvg + element.outerHTML;
        }
      }
      addIfAvailable(avatarDiv.querySelector('#skincolor').querySelector('.show'));
      addIfAvailable(avatarDiv.querySelector('#mouths').querySelector('.show'));
      addIfAvailable(avatarDiv.querySelector('#eyes').querySelector('.show'));
      addIfAvailable(avatarDiv.querySelector('#tattoos').querySelector('.show'));
      addIfAvailable(avatarDiv.querySelector('#facialhair2').querySelector('.show'));
      addIfAvailable(avatarDiv.querySelector('#eyebrows').querySelector('.show'));
      addIfAvailable(avatarDiv.querySelector('#accesories').querySelector('.show'));
      addIfAvailable(avatarDiv.querySelector('#clothes').querySelector('.show'));
      addIfAvailable(avatarDiv.querySelector('#hair').querySelector('.show'));
      addIfAvailable(avatarDiv.querySelector('#glasses').querySelector('.show'));


      combinedSvg = combinedSvg + '</svg>';
      console.log(combinedSvg);

      const canvas = document.createElement("canvas"); // create a canvas element
      canvas.width = 420;
      canvas.height = 420;
      const ctx = canvas.getContext('2d');
      const drawn = Canvg.fromString(ctx, combinedSvg, { ignoreClear: true, ignoreMouse: true });

      await drawn.render();

      const imageURL = canvas.toDataURL('image/png');
      const link = document.createElement('a');
      link.href = imageURL;
      link.download = 'avatar.png';
      document.body.appendChild(link);
      link.dispatchEvent(
          new MouseEvent('click', { 
            bubbles: true, 
            cancelable: true, 
            view: window 
          })
        );

      // Remove link from body
      document.body.removeChild(link);
    }
  }
}
</script>
