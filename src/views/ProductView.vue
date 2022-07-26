<template>
    <div class="profile">
        <h1>This is an product page</h1>
    </div>
    <div class="row">
        <div>
            <img :src="`${this.$route.params.image}`" alt="" class="product_img">
        </div>
        <div class="text">
            Looking for brand: <b>{{ this.$route.params.brand }}</b>
        </div>
        <div class="text">
            Looking for product: <b>{{ this.$route.params.product }}</b>
        </div>
        <div class="text">
            Looking for price: <b>{{ this.$route.params.price }}</b>
        </div>
        <div class="text">
            Looking for shop: <b>{{ this.$route.params.shop }}</b>
        </div>
    </div>
</template>


<style>
    .row{
        flex-direction: column;
        text-align: center;
        padding: 0px 100px 0px 100px;
    }
    .text{
        text-align: left;
    }
    .product_img{
        width: 200px;
        height: 200px;
        margin-bottom: 50px;
    }
</style>
