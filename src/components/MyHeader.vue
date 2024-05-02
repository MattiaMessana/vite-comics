<script>
    export default {
        data() {
            return {
                menu: [
                    {
                        title: "CHARACTERS",
                        status: false,
                    },
                    {
                        title: "COMICS",
                        status: true,
                    },
                    {
                        title: "MOVIES",
                        status: false,
                    },
                    {
                        title: "TV",
                        status: false,
                    },
                    {
                        title: "GAMES",
                        status: false,
                    },
                    {
                        title: "COLLECTIBLES",
                        status: false,
                    },
                    {
                        title: "VIDEOS",
                        status: false,
                    },
                    {
                        title: "FANS",
                        status: false,
                    },
                    {
                        title: "NEWS",
                        status: false,
                    },
                    {
                        title: "SHOP",
                        status: false,
                    },
                ],
            };
        },
    }
</script>

<template>
    <header>
        <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="DC COMICS LOGO">
        </div>
        <div class="links">
            <ul>
                <li v-for="curLink in menu"> 
                    <a href="" :class="{ active: curLink.status}"> {{curLink.title}}</a> 
                </li>
            </ul>
        </div>
    </header>
</template>

<style scoped lang="scss">
    @use "../style/partials/mixin" as *;
    @use "../style/partials/variables" as *; 

    header {
        background-color: $bg-header;
        @include flex(row, space-around , center);
        padding: 5px;
        
    }
    .logo {
        img {
            width: 80px;
            padding: 10px;
        }
    }

    .links {
        ul {
                @include flex(row, space-between, center);
                gap: 30px;
                list-style: none;
                    a {
                        color: $text-header;
                        text-decoration: none;
                            &:hover {
                                color: $primary-color;
                            }

                            &.active {
                                color: $primary-color;
                                border-bottom: 5px solid;
                                padding-bottom: 31.5px;
                            }
                        }

            }


        }
</style>