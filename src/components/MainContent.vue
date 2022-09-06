<template>
    <main>
     <div class="jumbo">

     </div>
     <div class="comics">
        <div class="container list">
             <ProductCard class="fumetti" v-for="(serie,index) in comics" :key="index" :src="serie.thumb" :title="serie=comics"/>
        </div>
        <div class="container cta">
            <a href="#"> LOAD MORE </a>
        </div>
     </div>
        
    </main>
    
</template>


<script>
import ProductCard from './ProductCard.vue';
import comics from '../dc-comics.js'

    export default {
    components: { 
        ProductCard 
    },
    data() {
        return {
            comics: comics
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
          .comics {
              padding: 3rem;
              color: white;
              background-color: black;
          }

          .list {
            display: flex;
            flex-wrap: nowrap; 
            margin-bottom: 50px;
          }
    }

</style>