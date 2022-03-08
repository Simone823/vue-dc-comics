// HTML
<template>

    <!-- Header -->
    <header>
        <!-- Container -->
        <div class="container">
            <!-- Logo  -->
            <figure class="logo">
                <img src="..\src\assets\img\dc-logo.png" alt="">
            </figure>
            <!-- Nav -->
            <nav class="menu">
                <ul>
                    <li v-for="(element, index) in menuLinks" :key="index">
                        <a :href="element.href">{{element.text}}</a>
                    </li>
                </ul>
            </nav>
        </div>

    </header>


</template>



// Javascript
<script>
export default {
    name: "MyHeader",

    data() {
        return {

            // Nav Links
            menuLinks: [
                {
                    href: "#",
                    text: "Characters", 
                },

                {
                    href: "#",
                    text: "Comics", 
                },

                {
                    href: "#",
                    text: "Movies", 
                },

                {
                    href: "#",
                    text: "Tv", 
                },

                {
                    href: "#",
                    text: "Games", 
                },

                {
                    href: "#",
                    text: "Collectibles", 
                },

                {
                    href: "#",
                    text: "Videos", 
                },

                {
                    href: "#",
                    text: "Fan", 
                },

                {
                    href: "#",
                    text: "News", 
                },

                {
                    href: "#",
                    text: "Shop", 
                },
            ],
        }
    },
}
</script>


// Stile scss valido solo per questo componenete
<style lang="scss" scoped>
header {
    padding: 5px 20px;

    .container {
        max-width: 1400px;
        margin: 0 auto;
        // border: 2px solid red;
        display: flex;
        align-items: center;
        justify-content: space-between;
        flex-wrap: wrap;
        row-gap: 20px;

        .logo {
            width: 82px;
            height: 82px;


            img {
                display: block;
                width: 100%;
            }
        }

        .menu ul {
            list-style: none;
            display: flex;
            gap: 20px;
            flex-wrap: wrap;
            

            a {
                text-decoration: none;
                color: currentColor;
                text-transform: uppercase;
                font-weight: 600;
            }
        }

    }
}

</style>