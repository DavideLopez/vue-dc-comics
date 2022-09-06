<template>
    <main>
     <div class="jumbo">

     </div>
     <div class="series">
        <div class="container list">
             <ProductCard class="fumetti" v-for="(serie,index) in series" :key="index" :src="serie.thumb" :title="serie=series"/>
        </div>
        <div class="container cta">
            <a href="#"> LOAD MORE </a>
        </div>
     </div>
        
    </main>
    
</template>


<script>
import ProductCard from './ProductCard.vue';
import series from '../dc-comics.js'

    export default {
    components: { 
        ProductCard 
    },
    data() {
        return {
            series: series
        }
    }
}
</script>

<style lang="scss" scoped>
    main {

       .jumbo {
         height: 400px;
         background: url('../assets/jumbotron.jpg');
       }
          .series {
              padding: 3rem;
              color: white;
              background-color: black;
          }

          .list {
            display: flex;
            flex-wrap: nowrap; 
            margin-bottom: 50px;
          }

          .fumetti {
            flex-basis: 185px;
            flex-grow: 1;
            padding: 0 0 10px;
          }

          .cta {
            text-align: center;

            a {
                padding: 12px 30px;
                line-height: 25px;
                background-color: #0282f9;
            }

            a:hover {
                opacity: 0.5;
            }
          }
    }

    

</style>