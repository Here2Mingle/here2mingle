<template>
  <div>
    <h3 class="channelHeader">Mingle Channels</h3>
    <ul class="nav nav-pills nav-justified mb-3" id="ex1" role="tablist">
      <li class="nav-item" role="presentation">
        <a class="nav-link active" id="ex3-tab-1" data-mdb-toggle="pill" href="#ex3-pills-1" role="tab"
          aria-controls="ex3-pills-1" aria-selected="true">Public</a>
      </li>
      <li class="nav-item" role="presentation">
        <a class="nav-link" id="ex3-tab-2" data-mdb-toggle="pill" href="#ex3-pills-2" role="tab"
          aria-controls="ex3-pills-2" aria-selected="false">Private</a>
      </li>
    </ul>
    <!-- Pills navs -->

    <!-- Pills content -->
    <div class="tab-content" id="ex2-content">
      <div class="tab-pane fade show active" id="ex3-pills-1" role="tabpanel" aria-labelledby="ex3-tab-1">
        <publicChannel />
      </div>
      <div class="tab-pane fade" id="ex3-pills-2" role="tabpanel" aria-labelledby="ex3-tab-2">
        <privateChannel />
      </div>
    </div>
  </div>
</template>

<script>
  import publicChannel from '~/components/channel/publicChannel.vue'
  import privateChannel from '~/components/channel/privateChannel.vue'

  export default {
    components: {
      publicChannel,
      privateChannel
    },
    head: {
      title: 'Mingle Channels'
    }
  }

</script>

<style>

</style>
