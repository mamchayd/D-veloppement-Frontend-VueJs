<template>
<webapp-slider/>
<webapp-best-places/>
<webapp-best-beach/>
<webapp-best-montain/>
<webapp-video/>
</template>

<script>
import Slider from './sections/Slider.vue';
import BestBeachSection from './sections/BestBeachSection.vue';
import BestMontainSection from './sections/BestMontainSection';
import BestPlacesSection from './sections/BestPlacesSection';
import Video from './sections/Video';
export default {
  name: 'Content',
  components: {
    'webapp-slider': Slider,
    'webapp-best-places': BestPlacesSection, 
    'webapp-best-beach': BestBeachSection,
    'webapp-best-montain': BestMontainSection,
    'webapp-video': Video
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
