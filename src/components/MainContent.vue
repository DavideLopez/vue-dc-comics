<template>
    <main>
        <div class="hero">
            <div class="container">
                <h2 class="hero-title">CURRENT SERIES</h2>
            </div>
        </div>
        <div class="series">
            <div class="container serie-list">
                <ProductCard class="serie-item" v-for="(serie, index) in series" :key="index" :src="serie.thumb" :title="serie.series" />
            </div>
            <div class="container cta">
                <a href="#">LOAD MORE</a>
            </div>
        </div>
    </main>
</template>

<script>
    import ProductCard from './ProductCard.vue';
    import series from '../dc-comics.js';

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
        .hero {
            background: url('../assets/jumbotron.jpg') top/cover no-repeat;
            background-color: #1c1c1c;

            .container {
                height: 400px;
                position: relative;
            }

            .hero-title {
                padding: 0.5rem 1rem;
                position: absolute;
                bottom: 0;
                left: 1rem;
                transform: translateY(+50%);
                background-color: #0282f9;
                color: #fff;
            }
        }

        .series {
            padding: 3rem 0;
            color: white;
            background-color: #1c1c1c;

            .serie-list {
                margin-bottom: 1.5rem;
                display: flex;
                flex-wrap: wrap;
                gap: 1.5rem;

                .serie-item {
                    flex-basis: 185px;
                    flex-grow: 1;
                    padding: 0 0.75rem;
                }
            }


            .cta {
                text-align: center;

                a {
                    display: inline-block;
                    padding: 10px 30px;
                    line-height: 25px;
                    background-color: #0282f9;
                    font-weight: bold;
                    
                    &:hover {
                        opacity: 0.5;
                    }
                }


            }
        }
    }
</style>