<template>
    <main>
        <!-- Jumbotron -->
        <section class="jumbotron">
            <div class="container">
                <button>Current Series</button>
            </div>
        </section>

        <!-- Contenuto parte centrale sfondo nero -->
        <section class="bkg-black">
            <!-- Container -->
            <div class="container">
                <h2>--> Content goes here</h2>
            </div>   
        </section>
    </main>
</template>



<script>
export default {
    name: "SectionBlack",  
}
</script>



<style lang="scss" scoped>

.jumbotron {
    width: 100%;
    height: 390px;
    background-image: url("../assets/img/jumbotron.jpg");
    background-repeat: no-repeat;
    background-position: top center;
    position: relative;
    padding: 0 20px;

    .container {
        max-width: 1400px;
        margin: 0 auto;

        button {
            padding: 10px 15px;
            color: white;
            background-color: #0282f9;
            border: none;
            position: absolute;
            bottom: 0;
            transform: translateY(50%);
            text-transform: uppercase;
        }
    }
}

.bkg-black {
    width: 100%;
    padding: 50px 20px;
    background-color: #1c1c1c;
    color: white;

    .container {
        max-width: 1400px;
        margin: 0 auto;
    }
}

</style>