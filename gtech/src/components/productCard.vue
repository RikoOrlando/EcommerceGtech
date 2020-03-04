<template>
    <div class="containerProductCard">
        <div>
            <img class="imageProduct" :src="data.url" alt="">
        </div>
        <div class="contentSale">
            <h3 class="productName fontStyle">{{data.title}}</h3>
            <p class="merk mT fontStyle">{{data.merk}}</p>
            <div class="mT">
                <i class="fas fa-star rate" v-for="(el, i) in data.rate" :key="i"></i>
            </div>
            <div class="priceWrap">
                <p class="priceBefore price fontStyle">{{data.priceBefore}}</p>
                <p class="priceAfter price fontStyle">{{data.priceAfter}}</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: ['data']

}
</script>

<style scoped>

.containerProductCard{
    background-color: white;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-left: 10px;
    margin-right: 10px
}

.imageProduct{
    width: 270px;
    height: 270px;
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
    color: rgb(61, 61, 61)
}

.fontStyle{
    font-family: Verdana, Geneva, Tahoma, sans-serif
}
</style>