<script>
export default {
    props: {
        cardImage: String,
        cardSeries: String,
    }
}
</script>

<template>
    <div class="card">
        <img :src="cardImage" :alt="cardSeries">
        <h5> {{ cardSeries }}</h5>
    </div>
</template>

<style scoped lang="scss">
     @use "../style/partials/mixin" as *;
    @use "../style/partials/variables" as *;

    card {
        @include flex (row, space-between, center);
        
    }

    img {
        width: 100px;
    }


    h5 {
        color: white;
        font-size: 15px;
        margin-top: 5px;
    }

</style>