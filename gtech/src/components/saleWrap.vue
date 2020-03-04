<template>
    <div>
        <div class="headSale">
            <h2 class="titleSale fontStyle">Sale</h2>
            <p class="childSale fontStyle">Lorem ipsum dolor sit amet consectetur</p>
        </div>
        <div class="containerSale">
            <product v-for="(el, i) in listSale" :key="i" :data="el"></product>
        </div>
    </div>
</template>

<script>
import product from './productCard'
export default {
    components: { product },
    data () {
        return {
            listSale: [
                    {
                        title: 'Green Shirt', 
                        rate: ['x','x','x'], 
                        url: 'https://www.brownsfashion.com/BWStaticContent/16000/16000/3426a7ea-67df-4b3e-b8f2-fc50bf31261c_jacquemus-model-in-floral-shirt.jpg', 
                        priceBefore: '$74.00', 
                        priceAfter: '$60.00', 
                        merk: 'H&M'
                    },
                    {
                        title: 'White Shirt', 
                        rate: ['x','x','x', 'x'], 
                        url: 'https://img1.cfcdn.club/5a/0a/5adb7a1b2e03d5d4e37ef055a184ca0a_350x350.jpg', 
                        priceBefore: '$100.00', 
                        priceAfter: '$70.00', 
                        merk: 'Uniqlo'
                    },
                    {
                        title: 'White Tshirt', 
                        rate: ['x','x','x','x','x'], 
                        url: 'https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcSIa8kdztQ8upO6NyP3AKxeAS97BPc58H1SmFEi-rpdKMiD8-OM', 
                        priceBefore: '$120.00', 
                        priceAfter: '$80.00', 
                        merk: 'Gucci'
                    }
                ]
        }
    }
}
</script>

<style scoped>

.containerSale{
    display: flex;
    width: 100%;
    justify-content: center;
    margin-bottom: 50px
}

.headSale{
    text-align: center
}

.titleSale{
    margin: 0%
}

.childSale{
    margin-top: 5px;
    color: gray
}

.fontStyle{
    font-family: Verdana, Geneva, Tahoma, sans-serif
}
</style>