<template>
  <section class="section">
      <div class="container is-clipped">
        <div id="bulmaCarousel">

          <div class="card" v-for="item in slideItems"  v-bind:key="item"> 
            <div class="card-image">
              <figure class="image is-3by1 is-covered">
                <img
                  :src="(item.img)"
                  alt=""
                />
              </figure>
            </div>
            <div class="card-content">
              <div class="item__title">
                {{item.title}}
              </div>
              <div class="item__description">
                {{item.description}}
                <span>Read more</span>
              </div>
            </div>
          </div>

        </div>
      </div>
    </section>

</template>
<script>
export default {
    name: "Slider",
    data: function(){
        return {
        slideItems:[]
        }
    },
    mounted: function() {
        // Initialize all elements with carousel class.

    },
    created: function() {
    this.slideItems = [{
            img:"./images/ouarzazate_sport.jpeg",
            title:'Un paradis de sable et de pierre',
            description:"Le plein de sensations fortes à la porte du désert !Vous avez envie de grands frissons dans un environnement de rêve ? Au cœur de la région de Ouarzazate, Zagora et Tinghir, vivez des moments intenses de sport : randonnée pédestre ou chamelière,... "
        },
        {
            img:"./images/Ahwach.jpeg",
            title:'Artisanat et traditions authentiques',
            description:"Les merveilles du Sud marocain! À l'est du pays, Ouarzazate, Zagora et Tinghir expriment la diversité culturelle du Maroc: elles témoignent des traditions les plus enracinées mais la création contemporaine n'est pas en reste en célébrant les plus grandes heures du cinéma!"
        },
        {
            img:"./images/ZAGORA-CHAMEAU.jpeg",
            title:'Ouarzazate, Au rythme du Sud',
            description:"Un voyage au coeur de la nature à Ouarzazate et ses environs ! Vous rêvez d'évasion au sein de paysages grandioses et dépaysants ? En compagnie d'un guide, parcourez les palmeraies du Drâa et de Skoura, les dunes de Tinfou, d'Erg Lihoudi ou encore de Chegaga et admirez la beauté ..."
        },
        {
            img:"./images/Morocco.jpeg",
            title:'Shopping et Artisanat traditionnel',
            description:"Le shopping aux abords du désert ! Acheter une multitude d'objets typiques tels que poteries, poignards et tapis, ou encore visiter leurs lieux de fabrication jusqu'à les confectionner soi-même, ce sont une partie des activités qui vous sont proposées à Ouarzazate, Zagora et Tinghir et ..."
        }];
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#bulmaCarousel .card .card-content{
    background: rgba(0, 0, 0, 0.4);
    width: 450px;
    height: 200px;
    position: absolute;
    bottom: 150px;
    right: 0px;
}
#bulmaCarousel .card .card-content * {
    color: #fff;
}
.item__title {
    font-size: 24px;
    font-weight: bold;
}
.item__description span{
    text-decoration: underline;
    font-weight: bold;
}
</style>
