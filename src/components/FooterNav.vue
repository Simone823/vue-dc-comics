<template>
    <!-- Footer nav -->
    <nav>
        <div class="container">
            <!-- Button -->
            <div class="button">
                <button>Sign-Up Now!</button>
            </div>

            <!-- Social -->
            <div class="social">
                <h2>{{titleSocial}}</h2>
                <ul>
                    <li v-for="(element, index) in arrayIconSocial" :key="index">
                        <a href="element.href"><img :src="require(`../assets${element.icon}`)" alt=""></a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>


<script>
export default {
    name: "FooterNav",
    data() {
        return {
            // Titolo div social
            titleSocial: "Follow Us",

            // Array Link e icone social
            arrayIconSocial: [
                {
                    href: "#",
                    icon: "/img/footer-facebook.png",
                },

                {
                    href: "#",
                    icon: "/img/footer-twitter.png",
                },

                {
                    href: "#",
                    icon: "/img/footer-youtube.png",
                },

                {
                    href: "#",
                    icon: "/img/footer-pinterest.png",
                },

                {
                    href: "#",
                    icon: "/img/footer-periscope.png",
                },
            ], 
        }
    }
}
</script>

<style lang="scss" scoped>
nav {
    background-color: #303030;
    padding: 25px 20px;

    .container {
        max-width: 1400px;
        margin: 0 auto;
        // border: 2px solid red;
        display: flex;
        align-items: center;
        justify-content: space-between;
        flex-wrap: wrap;
        row-gap: 20px;

        button {
            padding: 15px;
            text-transform: uppercase;
            background-color: transparent;
            color: white;
            border: 2px solid #0282f9;
            cursor: pointer;
        }

        .social {
            display: flex;
            align-items: center;
            gap: 30px;
            flex-wrap: wrap;

            h2 {
                color: #0282f9;
                text-transform: uppercase;
            }

            ul {
                list-style: none;
                display: flex;
                gap: 15px;
            }
        }
    }
}
</style>