<template>
  <a class="db center mw5 tc black link pa1"
     :title="`${plantData.commonName} - ${plantData.scientificName}`">
    <img v-if="plantData.image" class="db bg-white grow-3d"
         :alt="`${plantData.commonName} - ${plantData.scientificName}`"
         :src="require(`@/assets/images/${plantData.image}`)">

    <dl class="mt2 f6 lh-copy">
      <dt class="clip">{{ plantData.commonName }}</dt>
      <dd class="ml0">{{ plantData.scientificName }}</dd>
      <dt class="clip">{{ plantData.commonName }}</dt>
      <dd class="ml0 gray">{{ plantData.scientificName }}</dd>
    </dl>
  </a>
</template>

<script>
export default {
  name: 'PlantCard',
  props: {
    plantData: Object
  },
}
</script>

<style scoped lang="sass">

</style>