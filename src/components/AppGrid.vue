<template>
<section class="text-center">
    <h1>Lista Prodotti</h1>
     <div class="container px-4">
    <div class="row g-3 justify-content-center">
            <app-card class="col-6 col-sm-4 col-md-3" v-for="(product, index) in products" :key="index" :item="product"/>
        </div>
    </div>
</section>
    
</template>

<script>
import AppCard from './AppCard.vue'

export default {
    name: 'AppGrid', 
    components: { AppCard },
    
    data(){
        return {
            products: [
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/04/1-spaghetto-quadrato.jpg",
                titolo: "N.4 Spaghetto Quadrato Bucato",
                tipo: "lunga",
                cottura: 6,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/04/5-fettuccine.jpg",
                titolo: "N.5 Fettuccine",
                tipo: "lunga",
                cottura: 13,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/04/6-linguine.jpg",
                titolo: "N.6 Linguine",
                tipo: "lunga",
                cottura: 12,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/04/7-mezze-linguine.jpg",
                titolo: "N.7 Mezze Linguine",
                tipo: "lunga",
                cottura: 11,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/04/11-spaghettino-quadrato.jpg",
                titolo: "n.11 Spaghettino Quadrato",
                tipo: "lunga",
                cottura: 9,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/05/38-mezze-maniche.jpg",
                titolo: "N.38 Mezze maniche",
                tipo: "corta",
                cottura: 12,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/05/44-sedani.jpg",
                titolo: "N.44 Sedani",
                tipo: "corta",
                cottura: 8,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/05/49-sedani.jpg",
                titolo: "N.49 Sedanini",
                tipo: "corta",
                cottura: 8,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/05/53-lumachine.jpg",
                titolo: "N.53 Lumachine",
                tipo: "corta",
                cottura: 12,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/05/55-chifferi-rigati.jpg",
                titolo: "N.55 Chifferi rigati",
                tipo: "corta",
                cottura: 12,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/05/58-misto-corto.jpg",
                titolo: "N.58 Misto corto",
                tipo: "corta",
                cottura: 9,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/06/84-ditale-quadrato.jpg",
                titolo: "N.84 Ditale Quadrato",
                tipo: "cortissima",
                cottura: 12,
              },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/generals';
section{
    background-image:url('../assets/images/bg.jpg');
    background-size: cover;
}



</style>