<template>
   <div class="container">
      <div class="section food_card">
        
        <div class="card" v-for="item in bestPlces"  v-bind:key="item">
            <a href="">
            <div class="card-image">
                <figure class="image card_figure">
                <img 
                  :src="item.img"
                  :alt="item.title"                >
                </figure>
            </div>
            </a>
        </div>

      </div>
    </div>

</template>
<script>
export default {
    name: "BestPlacesSection",
    data: function(){
        return {
         bestPlces:[]
        }
    },
    mounted: function() {
        // Initialize all elements with carousel class.

    },
    created: function() {
        this.bestPlces = [{
            img:"./images/PALM-GOLF-Marrakech.jpeg",
            title:'PALM GOLF Marrakech'
        },
        {
            img:"./images/errqchidiq.jpeg",
            title:'Errachidia'
        },
        {
            img:"./images/Azilal-Beni_Mellal-khenifra-Office_tourisme_maroc-Office_tourisme_Azilal.jpeg",
            title:"zilal Beni Mellal"
        },
        {
            img:"./images/Plage-d'Al-Hoceima.jpeg",
            title:"Plage d'Al Hoceima"
        }];
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.card{
    box-shadow: none;
}

.card_figure img , .card_content{
  width: 400px;
  padding: 0;
}
.card_figure img , .card_content img{
  width: 400px;
  height: 200px;
}
.food_card {
    display: flex;
    padding: 0;
}
.food_card .card {
    margin-right: 10px;
}

</style>
