<template>
  <div>
    <img class="random download-img" @click="saveImage" :src="require('../assets/img/download.svg')">
  </div>
</template>

<script>
import Canvg from 'canvg';

export default {
  name: 'SaveImage',
  methods: {
    /**
     * This method creates an invisible anchor element which is automatically clicked
     * in order to download the image referenced by the URL passed to the method,
     *
     * @param {string} imageURL URL to the image to downloadя
     */
    downloadImage(imageURL) {
      // Creating an invisible anchor element and executing the 'click'
      // method seems to be the standard way of starting a download
      const downloadLink = document.createElement('a');
      downloadLink.href = imageURL;
      downloadLink.download = 'avatar.png';
      document.body.appendChild(downloadLink);
      downloadLink.dispatchEvent(
          new MouseEvent('click', { 
            bubbles: true, 
            cancelable: true, 
            view: window 
          })
        );

      // Remove link as final cleanup step
      document.body.removeChild(downloadLink);
    },
    /**
     * This method collects all _selected_ svg elements from the avatar
     * and renders them into a canvas using canvg.
     * Afterwards the image is provided as download to the user.
     */
    async saveImage() {
      // We need to have a single svg element which is passed to canvg
      let combinedSvg = '<div id="avatar" style="position:relative;width:100%;height:100%;"><svg width="360px" height="360px" viewBox="0 0 360 360" style="position: absolute;width: 100%;height: 100%;">';

      // Helper method to add only those group elements which actually exist
      // to the combined SVG string
      const addIfAvailable = (element) => {
        if (element !== undefined && element !== null) {
          combinedSvg = combinedSvg + element.outerHTML;
        }
      };


      // Select the visible group '<g>' from every option in the avatar
      // and add it to the combined SVG string.
      // Note: It would be shorter to use `avatarDiv.querySelectorAll('svg')` and iterate
      //       over these entries and their '<g>' groups. This does not work here though
      //       as we need to pay attention to the order of the elements to make sure nothing
      //       is hidden by another element.
      const avatarDiv = document.querySelector('#avatar');
      addIfAvailable(avatarDiv.querySelector('#skinColor').querySelector('.show'));
      addIfAvailable(avatarDiv.querySelector('#tattoos').querySelector('.show'));
      addIfAvailable(avatarDiv.querySelector('#accesories').querySelector('.show'));
      addIfAvailable(avatarDiv.querySelector('#clothes').querySelector('.show'));
      addIfAvailable(avatarDiv.querySelector('#eyebrows').querySelector('.show'));
      addIfAvailable(avatarDiv.querySelector('#eyes').querySelector('.show'));
      addIfAvailable(avatarDiv.querySelector('#mouths').querySelector('.show'));
      addIfAvailable(avatarDiv.querySelector('#hair').querySelector('.show'));
      addIfAvailable(avatarDiv.querySelector('#facialhair2').querySelector('.show'));
      addIfAvailable(avatarDiv.querySelector('#glasses').querySelector('.show'));

      combinedSvg = combinedSvg + '</svg></div>';

      // Create an invisible canvas and render the combined SVG onto the canvas.
      const canvas = document.createElement("canvas");
      canvas.width = 1200;
      canvas.height = 1200;
      const ctx = canvas.getContext('2d');
      const drawn = Canvg.fromString(ctx, combinedSvg);

      await drawn.render();

      this.downloadImage(canvas.toDataURL('image/png'));
    }
  }
}
</script>
