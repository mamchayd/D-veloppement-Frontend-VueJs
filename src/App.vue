<template>
<webapp-header/>
<webapp-content/>
<webapp-footer/>
</template>

<script>
import Header from './views/Header';
import Content from './components/Content';
import Footer from './views/Footer';
import bulmaCarousel from "bulma-carousel/dist/js/bulma-carousel.min.js";


export default {
  name: 'App',

  components: {
    'webapp-header':Header,
    'webapp-content':Content,
    'webapp-footer': Footer
  },

  data: () => ({
    //
  }),
  mounted: function () {
        new bulmaCarousel(document.getElementById("bulmaCarousel"));
    }
};
</script>