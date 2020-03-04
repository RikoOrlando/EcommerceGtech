<template>
    <div class="container">
        <div class="center">
            <div class="headLastest">
                <h2 class="fontFamily titleLast">Lastest Items</h2>
                <p class="fontFamily subTitleLast">Lorem ipsum dolor sit, amet consectetur adipisicing elit.</p>
            </div>
            <div class="wrap">
                <card v-for="(el, i) in newItem" :key="i" :data ="el"/>
            </div>
        </div>
    </div>
</template>

<script>
import card from './lastProductCard'
export default {
    components: {card},
    data() {
        return {
            newItem: [
                {title: '', url: 'https://asset-a.grid.id/crop/0x0:0x0/x/photo/2018/06/20/3133443698.jpg'}, 
                {title: '', url: 'https://image.made-in-china.com/2f0j00zsYtOZiRCcgJ/Latest-Fashion-Designs-Latest-Shirts-Pattern-Dress-Shirt-for-Men.jpg'}, 
                {title: '', url: 'https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRB7iM92KDxO2hjwM1H2XIgtu7VW-o_bgYZyEgORLZE0W7k0L_A'}
                ]
        }
    }
}
</script>

<style scoped>
.container{
    height: 700px;
    background-color: rgb(228, 226, 226);
    padding-top: 1%;
    padding-bottom: 1%
}

.wrap{
    display: flex;
    justify-content: center
}

.center{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100%;
    flex-direction: column;
}

.headLastest{
    text-align: center;
    /* margin-top: 40px */
}

.titleLast{
    margin-bottom: 0%
}

.fontFamily{
    font-family: Verdana, Geneva, Tahoma, sans-serif
}

.subTitleLast{
    margin-top: 0%;
    color: gray;
    /* margin-bottom: 40px */
}
</style>