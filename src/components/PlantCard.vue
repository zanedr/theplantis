<template>
  <a class="db center mw5 tc black link dim"
     :title="`${commonName} - ${latinName}`"
<!--     href="https://geo.itunes.apple.com/us/album/blonde/id1146195596?at=1l3vqFJ&mt=1&app=music"-->
  >

<!--    <img class="db ba b&#45;&#45;black-10"/-->
<!--    alt="Frank Ocean Blonde Album Cover"-->
<!--    src="https://s3-us-west-1.amazonaws.com/tachyonsio/img/Blonde-Frank_Ocean.jpeg"-->
<!--    >-->

    <dl class="mt2 f6 lh-copy">
      <dt class="clip">Title</dt>
      <dd class="ml0">Blonde</dd>
      <dt class="clip">Artist</dt>
      <dd class="ml0 gray">Frank Ocean</dd>
    </dl>
  </a>
</template>

<script>
export default {
  name: 'PlantCard',
  props: {
    commonName: String,
    latinName: String,
  }
}
</script>

<style>

</style>