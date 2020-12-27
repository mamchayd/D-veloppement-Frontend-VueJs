<template>
   <div class="container">
      <div class="section">
        <div class="card is-horizontal columns">
          <div class="card-image column is-three-fifths">

            <figure class="image is-2by1">
              <img  v-bind:src="beachImg" 
              alt="this used to be photo">             
            </figure>
          </div>
          <div class="card-content column is-two-fifths">
            <div class="media">
              <div class="media-content">
                <p class="title">{{title}}</p>
              </div>
            </div>

            <div class="content">
              {{description}}
              <br/>
              <a href="#" class="read_more"><span class="tag is-info">Read more</span></a>
            </div>
          </div>
        </div>
  </div>
        </div>

</template>
<script>
export default {
    name: "BestBeachSection",
    data: function(){
        return {
        beachImg:"",
        title: "",
        description:""
        }
    },
    mounted: function() {
        // Initialize all elements with carousel class.

    },
    created: function() {
        this.beachImg = './images/dakhla.png';
        this.title = "Une lagune mythique";
        this.description = "Jouez les Robinson Crusoé sur les plages de Dakhla Du nord au sud, avec ses centaines de kilomètres de plages de sable fin et désertes, s’ouvrant sur l’Atlantique, Dakhla vous offre un décor sublime. Vous vous sentirez en symbiose avec une nature aussi mystérieuse que préservée. Située sur une presque île, à l’embouchure du Rio de Oro, la baie de Dakhla et sa splendide lagune aux eaux chaudes et turquoise abritent oiseaux migrateurs, flamands roses, tortues, phoques moines, raies et dauphins à bosse. Vous pourrez les admirer depuis l’extrémité sud de la presqu’île, à Punta Sarga. ";
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>


.card{
    box-shadow: none;
}

.card-content .content {
    line-height: 1.5;
    font-size: 18px;
}

</style>
