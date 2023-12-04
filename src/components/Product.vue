<template>
    <div class="product">
        <div class="image"><img :src="getImagePath()" alt=""></div>
        <div class="title">{{ title }}</div>
        <div class="price">
            <div class="price-normal">2499т</div>
            <div class="price-discount">1990т</div>
        </div>
        <div class="add"><a href="#">Добавить в корзину</a></div>
    </div>
</template>

<script>
export default {
    name: 'ProductComponent',
    props: {
        imageId: Number,
        title: String
    },
    methods: {
        getImagePath() {
            return require("../assets/products/" + this.imageId + '.png');
        }
    },
}
</script>

<style scoped>
.product {
    width: 279px;
    height: 468px;
    border: 2px solid #DD926E;
    border-radius: 24px;
    box-sizing: border-box;
    padding-top: 55px;
    padding-left: 30px;
    padding-right: 30px;
}

.product:hover {
    background-color: #FFE5D9;
    border: none;
    box-sizing: border-box;
}

.image {
    width: 200px;
    height: 200px;
    margin: 0 auto;
}

.title {
    margin-top: 38px;
    text-align: center;
    font-size: 15px;
    color: #CF6736;
}

.price {
    margin-top: 20px;
}

.price-normal {
    color: #DD926E;
    font-size: 16px;
    text-decoration: line-through;
    text-align: center;
}

.price-discount {
    color: #CF6736;
    font-size: 24px;
    text-align: center;
}

.add {
    margin-top: 20px;
    font-size: 16px;
    text-align: center;
}

a {
    text-decoration: none;
    color: #DD926E;
}
</style>

