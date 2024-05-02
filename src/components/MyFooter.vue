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

        </div>
    </footer>
</template>

<style scoped lang="scss">
    @use "../style/partials/mixin" as *;
    @use "../style/partials/variables" as *; 

.links {
    background-image: url(../assets/img/footer-bg.jpg);
    @include flex(row, flex-start , center);
    padding: 10px;
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


</style>