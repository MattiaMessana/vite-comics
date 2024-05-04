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


</style>