<template>
  <div>
    <video ref="videoPlayer" class="video-js"></video>
  </div>
</template>

<script>
  import videojs from 'video.js';

  export default {
    name: 'VideoPlayer',
    props: {
      options: {
        type: Object,
        default () {
          return {};
        }
      }
    },
    data() {
      return {
        player: null
      }
    },
    mounted() {
      var shareOptions = {
        socials: ['fb', 'tw', 'reddit', 'gp', 'messenger', 'linkedin', 'telegram', 'whatsapp', 'viber', 'vk', 'ok',
          'mail'
        ],

        url: window.location.href,
        title: 'videojs-share',
        description: 'video.js share plugin',
        image: 'https://dummyimage.com/1200x630',

        // required for Facebook and Messenger
        fbAppId: '12345',
        // optional for Facebook
        redirectUri: window.location.href + '#close',

        // optional for VK
        isVkParse: true,

        // optinal embed code
        embedCode: '<iframe src="' + window.location.href +
          '" width="560" height="315" frameborder="0" allowfullscreen></iframe>'
      }
      this.player = videojs(this.$refs.videoPlayer, this.options, () => {
        this.player.log('onPlayerReady', this);
        player.responsive(true);
        player.straasLiveEventListener();
        player.share(shareOptions);
      });
    },
    beforeDestroy() {
      if (this.player) {
        this.player.dispose();
      }
    }
  }

</script>
