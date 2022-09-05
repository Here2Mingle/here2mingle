<template>
    <div>
        <video src="" controls id="gamePlay"></video>
        <RelatedGames />
    </div>
</template>

<script>
import RelatedGames from '~/components/RelatedGames.vue'

export default {
    components: {RelatedGames},
    head: {
        title: ''
    }
}
</script>

<style>

</style>