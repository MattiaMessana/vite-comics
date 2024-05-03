<script>
    export default {
        data() {
            return {

            }
        }
    }
</script>

<template>
    <footer>
        <div class="container">

            <div class="links">
                <ul>
                    <p class="title">DC COMICS</p>
                    <li> <a href="">Characteres</a></li>
                    <li><a href="">Comics</a></li>
                    <li><a href="">Movies</a></li>
                    <li><a href="">TV</a></li>
                    <li><a href="">Games</a></li>
                    <li><a href="">Videos</a></li>
                    <li><a href="">News</a></li>

                    <p class="title">DC</p>
                    <li><a href="">Terms Of Use</a></li>
                    <li><a href="">Privacy policy (New)</a></li>
                    <li><a href="">Ad Choices</a></li>
                    <li><a href="">Adversting</a></li>
                    <li><a href="">Jobs</a></li>
                    <li><a href="">Subscriptions</a></li>
                    <li><a href="">Talent Workshops</a></li>
                    <li><a href="">CPSC Certificates</a></li>
                    <li><a href="">Ratings</a></li>
                    <li><a href="">Shop Help</a></li>
                    <li><a href="">Contact Us</a></li>

                </ul>
            </div>

            <div class="sign-up">
                <button> SIGN-UP NOW </button>
            </div>

        </div>
    </footer>
</template>

<style scoped lang="scss">
    @use "../style/partials/mixin" as *;
    @use "../style/partials/variables" as *;

    /* .container {
        width: 80%;
        margin: 0 auto;
    } */
    .links {
        background-image: url(../assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-position: center;
        background-size: cover;
        padding: 10px;
        @include flex(row, flex-start, center);

        .title {
            color: white;
        }

        li {
            list-style-type: none;

            a {
                text-decoration: none;
                color: $text-footer;
            }
        }

        p {
            font-size: 1.4rem;
            margin-bottom: 10px;
        }
    }

    .sign-up {
        background-color: $bg-footer ;
        padding: 20px;

        button {
            border: 2px solid;
            border-color: $primary-color;
            padding: 10px;
            background-color: $bg-footer ;
            color: white;
            cursor: pointer;

        }
    }
</style>