<script>
import MyProductCards from "./MyProductCards.vue";
import productsList from "../assets/data/DataProducts.js";

    export default {
        components: {
            MyProductCards,
        },
        data() {
            return {
                products: productsList,
            }
        }
    }
</script>

<template>

<main>
    <section>
        <img src="../assets/img/jumbotron.jpg" alt="">
        <button>CURRENT SERIES</button>
    </section>

   <div class="row">
    <div class="col" v-for="curProd in products">
        <MyProductCards
            :cardImage="curProd.thumb"
            :cardSeries="curProd.series"
        />
    </div>
   </div>
</main>

</template>

<style lang="scss" scoped>
    @use "../style/partials/mixin" as *;
    @use "../style/partials/variables" as *;


</style>