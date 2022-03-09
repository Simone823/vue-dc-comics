<template>
    <main>
        <!-- Jumbotron -->
        <section class="jumbotron">
            <img src="../assets/img/jumbotron.jpg" alt="">
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

    img {
        width: 100%;
        height: 100%;
        display: block;
        object-fit: cover;
        object-position: top center;
    }
}

.bkg-black {
    width: 100%;
    // padding: 50px 20px;
    background-color: #1c1c1c;
    color: white;

    .container {
        max-width: 1400px;
        margin: 0 auto;
    }
}

</style>