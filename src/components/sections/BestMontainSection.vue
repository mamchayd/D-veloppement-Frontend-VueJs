<template>
   <div class="container">
      <div class="section">
        <div class="card is-horizontal columns">

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
          <div class="card-image column is-three-fifths">

            <figure class="image is-2by1">
              <img  v-bind:src="beachImg" 
              alt="this used to be photo">             
            </figure>
          </div>
        </div>
      </div>
    </div>

</template>
<script>
export default {
    name: "BestMontainSection",
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
        this.beachImg = './images/eco-lodge.jpeg';
        this.title = "Destinations vertes et montagnes";
        this.description = "Une montagne à tout faire ! Le Maroc est un pays que parcourent les montagnes. Les trois Atlas et le Rif composent de merveilleux paysages escarpés mais aussi ils font d'authentiques terrains de jeu pour tous les amateurs d'aventure ! La randonnée et le trek sont des activités prisées. Nombre de ces promenades sportives prennent pied parmi les parcs naturels du pays: à proximité de Chefchaouen dans le Parc National de Talassemtane ou encore non loin d'Ifrane, dans le parc national du même nom. Dans les environs de Marrakech, l'ascension du Mont Toubkal est un incontournable.";
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.card{
    box-shadow: none;
}

.card_figure img , .card_content{
  width: 300px;
  padding: 0;
}
.card-content .content {
    line-height: 1.5;
    font-size: 18px;
}
</style>
