<template>

    <!-- Footer -->
    <footer>

        <!-- Container -->
        <div class="container">
            <!-- Wrapper list -->
            <div class="wrapper">

                <!-- Lista ul 1  -->
                <div class="list-1-wrapper">
                    <h1>{{title1}}</h1>
                    <ul>
                        <li v-for="(element, index) in arrayLink1" :key="index">
                            <a href="element.href">{{element.link}}</a>
                        </li>
                    </ul>

                    <!-- Lista ul 2 -->
                    <h1>{{title2}}</h1>
                    <ul>
                        <li v-for="(element, index) in arrayLink2" :key="index">
                            <a href="element.href">{{element.link}}</a>
                        </li>
                    </ul>
                </div>

                <!-- Lista ul 2 -->
                <div class="list-2-wrapper">
                    <h1>{{title3}}</h1>
                    <ul>
                        <li v-for="(element, index) in arrayLink3" :key="index">
                            <a href="element.href">{{element.link}}</a>
                        </li>
                    </ul>
                </div>

                <!-- Lista ul 3 -->
                <div class="list-3-wrapper">
                    <h1>{{title4}}</h1>
                    <ul>
                        <li v-for="(element, index) in arrayLink4" :key="index">
                            <a href="element.href">{{element.link}}</a>
                        </li>
                    </ul>
                </div>
            </div>

            <!-- Wrapper Logo -->
            <div class="wrapper logo_dc">

            </div>

        </div>
    </footer>

</template>


<script>
export default {
    name: "MyFooter",
    data() {
        return{

            // Titolo lista ul 1
            title1: "Dc Comics",

            // Titolo lista ul 2
            title2: "Shop",

            // Titolo lista ul 3
            title3: "Dc",

            // Titolo lista ul 4
            title4: "Sites",

            // Array Link 1
            arrayLink1: [
                {
                    href: "#",
                    link: "Characters",
                },

                {
                    href: "#",
                    link: "Comics",
                },

                {
                    href: "#",
                    link: "Movies",
                },

                {
                    href: "#",
                    link: "TV",
                },

                {
                    href: "#",
                    link: "Games",
                },

                {
                    href: "#",
                    link: "Videos",
                },

                {
                    href: "#",
                    link: "News",
                },
            ],

            // Array Link 2
            arrayLink2: [
                {
                    href: "#",
                    link: "Shop DC",
                },

                {
                    href: "#",
                    link: "Shop DC Collectibles",
                },
            ],

            // Array Link3
            arrayLink3: [
                {
                    href: "#",
                    link: "Terms Of Use",
                },

                {
                    href: "#",
                    link: "Terms Of Use",
                },

                {
                    href: "#",
                    link: "Privacy policy (New)",
                },

                {
                    href: "#",
                    link: "Ad Choise",
                },

                {
                    href: "#",
                    link: "Advertising",
                },

                {
                    href: "#",
                    link: "Jobs",
                },

                {
                    href: "#",
                    link: "Subscriptions",
                },

                {
                    href: "#",
                    link: "Talent Workshops",
                },

                {
                    href: "#",
                    link: "CPSC Certificates",
                },

                {
                    href: "#",
                    link: "Ratings",
                },

                {
                    href: "#",
                    link: "Shop Help",
                },

                {
                    href: "#",
                    link: "Contact Us",
                },
            ],

            // Array Link 4
            arrayLink4: [
                {
                    href: "#",
                    link: "DC",
                },

                {
                    href: "#",
                    link: "MAD Magazine",
                },

                {
                    href: "#",
                    link: "DC Kids",
                },

                {
                    href: "#",
                    link: "DC Universe",
                },

                {
                    href: "#",
                    link: "DC Power Visa",
                },
            ],


        }
    }
    
}   
</script>




<style lang="scss" scoped>
footer {
    width: 100%;
    // height: 370px;
    background-image: url("../assets/img/footer-bg.jpg");
    padding: 0 20px;

    .container {
        max-width: 1400px;
        margin: 0 auto;
        // border: 2px solid red;
        display: flex;
        flex-wrap: wrap;

        .wrapper {
            // border: 2px solid orange;
            flex-basis: calc(100% / 2);
            color: white;
            padding: 40px 20px;
            display: flex;
            gap: 30px;
            flex-wrap: wrap;

            .list-1-wrapper {
                display: flex;
                flex-direction: column;
                gap: 25px;

                h1 {
                    text-transform: uppercase;
                    font-size: 20px;
                }

                ul {
                    list-style: none;

                    li {
                        padding-bottom: 10px;
                    }

                    a {
                        text-decoration: none;
                        color: #aaa;
                    }
                }
            }

            .list-2-wrapper {
                display: flex;
                flex-direction: column;
                gap: 25px;

                h1 {
                    text-transform: uppercase;
                    font-size: 20px;
                }

                ul {
                    list-style: none;

                    li {
                        padding-bottom: 10px;
                    }

                    a {
                        text-decoration: none;
                        color: #aaa;
                    }
                }
            }

            .list-3-wrapper {
                display: flex;
                flex-direction: column;
                gap: 25px;

                h1 {
                    text-transform: uppercase;
                    font-size: 20px;
                }

                ul {
                    list-style: none;

                    li {
                        padding-bottom: 10px;
                    }

                    a {
                        text-decoration: none;
                        color: #aaa;
                    }
                }
            }

        }

        .logo_dc {
            background-image: url("../assets/img/dc-logo-bg.png");
            background-repeat: no-repeat;
            background-position: center right;
            flex-shrink: 0;
        }
    }
}

</style>