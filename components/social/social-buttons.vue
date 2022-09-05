<template>
  <div class="bubblesPanel">
    <div class="lightbox">
      <div class="row">
        <div class="col-md-3">
          <button type="button" class="btn btn-primary fas fa-plus" data-mdb-toggle="modal" data-mdb-target="#exampleModal" style="font-size: 30px;"></button>
        </div>
        <div class="col-md-3">
          <img class="rounded-bubbles shadow-1-strong"
            src="https://mdbootstrap.com/img/Photos/Lightbox/Original/img%20(69).jpg"
            data-mdb-img="https://mdbootstrap.com/img/Photos/Lightbox/Original/img%20(69).jpg" alt="avatar"
            style="width: 105px;" />
        </div>

        <div class="col-md-3">
          <img class="rounded-bubbles shadow-1-strong"
            src="https://mdbootstrap.com/img/Photos/Lightbox/Original/img%20(67).jpg"
            data-mdb-img="https://mdbootstrap.com/img/Photos/Lightbox/Original/img%20(67).jpg" alt="avatar"
            style="width: 105px;" />
        </div>

        <div class="col-md-3">
          <img class="rounded-bubbles shadow-1-strong"
            src="https://mdbootstrap.com/img/Photos/Lightbox/Original/img%20(72).jpg"
            data-mdb-img="https://mdbootstrap.com/img/Photos/Lightbox/Original/img%20(72).jpg" alt="avatar"
            style="width: 105px;" />
        </div>
      </div>
    </div>
    <record />
  </div>
</template>

<script>
import record from '~/components/social/record'

export default {
  
  components: {
      record,
  }
}

</script>
