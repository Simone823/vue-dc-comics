<template>

    <!-- Sezione con sfondo azzurro -->
    <section class="bkg-blue">
        <!-- Container -->
        <div class="container">
            <ul>
                <li v-for="(element, index) in menuLinks" :key="index">
                    <figure class="logo">
                        <img :src="require(`../assets${element.img}`)" alt="">
                    </figure>
                    <a :href="element.href">{{element.text}}</a>
                </li>
            </ul>
        </div>
    </section>

</template>


<script>
export default {
    name: "SectionBlue",
    data() {
        return {

            // Array menu link
            menuLinks: [
                {
                    img: "/img/buy-comics-digital-comics.png",
                    href: "#",
                    text: "Digital Comics",
                },

                {
                    img: "/img/buy-comics-merchandise.png",
                    href: "#",
                    text: "Dc Merchandise",
                },

                {
                    img: "/img/buy-comics-shop-locator.png",
                    href: "#",
                    text: "Subscription",
                },

                {
                    img: "/img/buy-comics-subscriptions.png",
                    href: "#",
                    text: "Comic Shop Locator",
                },

                {
                    img: "/img/buy-dc-power-visa.svg",
                    href: "#",
                    text: "Dc Power Visa",
                },
            ],
        }
    }
    
}
</script>


<style lang="scss" scoped>
.bkg-blue {
    background-color: #0282f9;
    padding: 50px 20px;

    .container {
        max-width: 1400px;
        padding: 0 25px;
        margin: 0 auto;
        display: flex;
        flex-wrap: wrap;
        gap: 20px;
        row-gap: 30px;
    
        
        ul {
            display: contents;
        }

        li {
            list-style: none;
            display: flex;
            align-items: center;
            gap: 20px;
            flex-basis: calc(100% / 5 - 20px);
            flex-shrink: 0;
            padding: 0 10px;

            .logo {
                width: 45px;

                img{
                    width: 100%;
                    display: block;
                    object-fit: contain;
                }
            }

            a {
                text-decoration: none;
                color: white;
                text-transform: uppercase;
                font-size: 16px;
            }
        }
    }

}

</style>