<template>

    <!-- Card -->
    <div class="card">
        <img :src="thumb">
        <p class="series">{{series}}</p>
        <p class="type">{{type}}</p>
        <p class="price">{{price}}</p>
    </div>

</template>



<script>
export default {
    name: "ListCard",

    props: {
        thumb: String,
        series: String,
        type: String,
        price: String,
    }
    
}
</script>


<style lang="scss" scoped>
.card {
    flex-basis: calc(100% / 6 - 20px);
    flex-shrink: 0;
    
    img {
        width: 100%;
        aspect-ratio: 1;
        object-fit: cover;
        object-position: top;
        display: block;
        margin-bottom: 18px;
    }

    .series {
        text-transform: uppercase;
        margin-bottom: 5px;
    }

    .type {
        font-size: 12px;
        color: #aaa;
        margin-bottom: 4px;
    }

    .price {
        font-size: 12px;
        color: #aaa;
        text-decoration: line-through;
    }
}

</style>