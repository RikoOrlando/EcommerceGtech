<template>
    <div>
        <hr>
        <div class="containerProductCard">
            <div>
                <img class="imageProduct" :src="data.url" alt="">
            </div>
            <div class="contentSale">
                <h3 class="productName">{{data.title}}</h3>
                <p class="merk mT">{{data.merk}}</p>
                <div class="mT">
                    <i class="fas fa-star rate"></i>
                    <i class="fas fa-star rate"></i>
                    <i class="fas fa-star rate"></i>
                    <i class="fas fa-star rate"></i>
                    <i class="fas fa-star rate"></i>
                </div>
                <div class="priceWrap">
                    <p class="priceBefore price">{{data.beforePrice}}</p>
                    <p class="priceAfter price">{{data.afterPrice}}</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: ['data'],
}
</script>

<style scoped>

.containerProductCard{
    background-color: white;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    margin-left: 10px;
    margin-right: 10px
}

.imageProduct{
    width: 130px;
    height: 160px;
}

.priceWrap{
    display: flex;
    justify-content: center
}

.priceBefore{
    color: grey;
    text-decoration-line: line-through;
    margin-right: 10px
}

.priceAfter{
    font-weight: bold;
    color: red
}

.rate{
    color: gold;
    font-size: 15px
}

.price{
    margin-top: 2px
}

.contentSale{
    text-align: center
}

.productName{
    margin: 0%;
    margin-top: 10px
}

.mT{
    margin-top: 0px;
    margin-bottom: 10px
}

.merk{
    color: grey
}
</style>