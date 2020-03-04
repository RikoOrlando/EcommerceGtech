<template>
    <carousel :autoplay="true" :nav="false" :dots="false" :mergeFit="false" :autoWidth="true" :autoHeight="true" :autoplayTimeout="2000">
        <div class="page">
            <img src="https://blog.celect.com/hs-fs/hubfs/delivery-ecommerce-banner.png?width=1200&name=delivery-ecommerce-banner.png">
        </div>
        <div class="page">
            <img src="https://previews.123rf.com/images/gmast3r/gmast3r1608/gmast3r160800729/61287943-online-shopping-banner-ecommerce-concept-flat-vector-illustration.jpg">
        </div>
        <div class="page">
            <img src="https://www.planetwebsolution.com/blog/wp-content/uploads/2016/06/blog-banner-big-1.jpg">
        </div>
        <div class="page">
            <img src="https://cdna.artstation.com/p/assets/images/images/023/648/044/large/tanaya-dutta-x-e-commerce-banner-option-2.jpg?1579881041">
        </div>
    </carousel>
</template>

<script>
import carousel from 'vue-owl-carousel2'
export default {
    components: {carousel}
}
</script>

<style scoped>
.page{
    height: 60vh;
    background: red;
    width: 100vw;
    display: flex;
    justify-content: center;
    align-items: center

}

</style>