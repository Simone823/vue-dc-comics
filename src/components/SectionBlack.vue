<template>

    <!-- Contenuto parte centrale sfondo nero -->
    <section class="bkg-black">
        <!-- Container -->
        <div class="container">
            <h2>--> Content goes here</h2>
        </div>   
    </section>

</template>



<script>
export default {
    name: "SectionBlack",  
}
</script>



<style lang="scss" scoped>

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