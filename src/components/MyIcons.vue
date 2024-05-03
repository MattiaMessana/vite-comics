<script>
    export default {
        data() {
            return {
                icons: [
                    {
                        title: "DIGITAL COMICS",
                        image: "buy-comics-digital-comics.png",
                    },
                    {
                        title: "DC MERCHANDISE",
                        image: "buy-comics-merchandise.png",
                    },
                    {
                        title: "SUBSCRITION",
                        image: "buy-comics-subscriptions.png",
                    },
                    {
                        title: "COMIC SHOP LOCATOR",
                        image: "buy-comics-shop-locator.png",
                    },
                    {
                        title: "DC POWER VISA",
                        image: "buy-dc-power-visa.svg",
                    },
                ]
            }
        },
        methods: {
            getImagePath: function(imageName) {
                return new URL(`../assets/img/${imageName.image}`, import.meta.url).href;
            }
        }
    }
</script>

<template>
   <section>
    <div class="icon" v-for="curIcon in icons">
        <img :src="getImagePath(curIcon)" :alt="curIcon.title">
        <!-- <img src="../assets/img/buy-comics-digital-comics.png" alt=""> -->
        <p> {{ curIcon.title }} </p>
    </div>
   </section>
</template>

<style scoped lang="scss">
    @use "../style/partials/mixin" as *;
    @use "../style/partials/variables" as *; 

    section {
        background-color: $primary-color;
        padding: 20px;
        @include flex(row, space-between, center);
        color: white;
    }

    .icon {
        @include flex(row, space-between, center);
        padding: 10px;
        margin-left: 20px;
        margin-right: 20px;
        img {
            // width: 40px;
            height: 50px;
        }
        p {
            margin-left: 5px;
            font-size: .8rem;
        }
    }

</style>