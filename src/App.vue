<template>
  <section id="app" class="fl w-90">
    <header class="relative bg-white z-2 fixed w-100 h4 ph3 pv3 pv4-ns ph4-m ph5-l">
<!--      <nav class="f6 fw6 ttu tracked">-->
<!--        <a class="link dim white dib mr3" href="#" title="Home">Home</a>-->
<!--        <a class="link dim white dib mr3" href="#" title="About">About</a>-->
<!--        <a class="link dim white dib mr3" href="#" title="Store">Store</a>-->
<!--        <a class="link dim white dib" href="#" title="Contact">Contact</a>-->
<!--      </nav>-->
      <p class="ttu tc inconsolata font-green">09.23.20</p>
      <p class="ttu tc inconsolata font-green">This is The Plant Site the data base of my plants and how I care for them.</p>
    </header>
    <span class="flex flex-wrap justify-start pa5 mt5" v-if="plantsArray.length">
        <plant-card v-for="(plant, index) in plantsArray"
                    :key="index"
                    :plant-data="plant"></plant-card>
    </span>
  </section>
</template>

<script>
import PlantCard from "@/components/PlantCard";
import { plantsArray } from "@/stubData/plantData";

export default {
  name: 'App',
  components: {
    PlantCard,
  },
  data() {
    return {
      plantsArray: plantsArray
    }
  }
}
</script>

<style lang="scss">
@import './styles/custom.scss';

#app {
  width: 100%;
  height: 100%;
}
</style>
