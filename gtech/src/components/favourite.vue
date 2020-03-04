<template>
  <div class="containerFav">
      <div class="favouriteWrap">
          <div class="subWrap">
                <div>   
                        <h3 class="cnter">Our Brands</h3>
                        <favCard v-for="(el, i) in favOne" :key="i" :data="el"></favCard>
                </div>
                <div>
                    <img class="imageMiddle" src="https://image.freepik.com/free-vector/different-elements-online-shopping_1085-848.jpg" alt="">
                </div>
                <div>
                        <h3 class="cnter">Our Brands</h3>
                        <favCard v-for="(el, i) in favTwo" :key="i" :data="el"></favCard>
                </div>
          </div>
          <div class="break"></div>
          <div class="searchWrap">
                <div>
                <h3 class="titleInput"> Never Miss any fashion tranding</h3>
                <p class="subTitle">Lorem ipsum dolor sit, amet consectetur adipisicing elit</p>
                </div>
                <div>
                    <input class="inpt" type="text">
                    <button class="button">Search</button>
                </div>
          </div>
      </div>
  </div>
</template>

<script>
import favCard from './favouriteCard'
export default {
    components: {favCard},
    data () {
        return {
            favOne: [
                    {
                        title: 'Black Dress',
                        merk: 'Guess',
                        beforePrice: '$100.00',
                        afterPrice: '$70.00',
                        url: 'https://static.topshop.com/v1/static/json-0000156327_Denim_WK26jpg'
                    },
                    {
                        title: 'Blue Jeans',
                        merk: 'H&M',
                        beforePrice: '$70.00',
                        afterPrice: '$50.00',
                        url: 'https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQKfBauArZnNDGByYgW9wKmA3rlHXaPqexskW5XfpY5QtCQUqbc'
                    },
                    {
                        title: 'Chino Pants',
                        merk: 'Levis',
                        beforePrice: '$100.00',
                        afterPrice: '$80.00',
                        url: 'https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRNIs6Mu45-xuEWlhivSER_T3WTOaWj-Nj9Aw0ZT_PuAa8ypGdb'
                    },
                    {
                        title: 'Sweet Sweater',
                        merk: 'Gucci',
                        beforePrice: '$90.00',
                        afterPrice: '$70.00',
                        url: 'https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcSxuWxcB2meqnn7PHUDlTIBMUCNChY-ZL7PE4445_jXxwwcwDSm'
                    }
                ],
            favTwo: [
                    {
                        title: 'Black Pants',
                        merk: 'Zara',
                        beforePrice: '$70.00',
                        afterPrice: '$60.00',
                        url: 'https://media.thereformation.com/image/upload/q_auto:eco/c_scale,w_auto:breakpoints_100_1920_9_20:546/v1/prod/media/W1siZiIsIjIwMjAvMDMvMDIvMTcvMjkvNDYvZDQ1MDUzMzgtMmE0ZC00OTdmLWE5MWYtY2IyYjc4ZTUxOGYxL1NUUkVUQ0hfRkxPT0RfSkVBTl9CTEFDSy5qcGciXV0/STRETCH_FLOOD_JEAN_BLACK.jpg'
                    },
                    {
                        title: 'Cool Jacket',
                        merk: 'H&M',
                        beforePrice: '$75.00',
                        afterPrice: '$50.00',
                        url: 'https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQ4QsztSQrSebfoTFAESouWa9GuQ0u0rXDV7khsj1_RpHdwgP5S'
                    },
                    {
                        title: 'Shirt',
                        merk: 'Levis',
                        beforePrice: '$100.00',
                        afterPrice: '$70.00',
                        url: 'https://imagesvc.meredithcorp.io/v3/mm/image?url=https%3A%2F%2Fcdn-img.instyle.com%2Fsites%2Fdefault%2Ffiles%2Fstyles%2F640x768%2Fpublic%2F1582145992%2Finstant-style.jpg%3Fitok%3DuaeH5sWs'
                    },
                    {
                        title: 'Long Dress',
                        merk: 'Guess',
                        beforePrice: '$85.00',
                        afterPrice: '$70.00',
                        url: 'https://www3.next.co.uk/nxtcms/resource/image/2738390/portrait_ratio5x7/300/420/6377ebcfa7336c3f57bdb060e06cabb4/aX/womens-dresses.jpg'
                    }
                ],
        }
    }
}
</script>

<style scoped>
.containerFav{
    background: url('https://www.rapormerah.co/wp-content/uploads/2017/08/geometic-bg-white-3.jpg');
    height: 900px;
    display: flex;
    justify-content: center;
    align-items: center
}

.favouriteWrap{
    background-color: white;
    height: 110%;
    width: 65%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center
}

.imageMiddle{
    height: 400px;
    width: 350px
}

.subWrap{
    display: flex;
    align-items: center
}

.button{
    height: 35px;
    width: 100px;
    background: #EE4F4C;
    color: white;
    border: none;
    font-weight: bold;
    cursor: pointer;
}

.inpt{
    height: 30px;
    width: 400px;
    margin-right: 10px;
    background: white;
    border: none;
    border-bottom: 1px solid black
}

.searchWrap{
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center
}

.titleInput{
    margin-bottom: 0%;
    text-align: center
}

.subTitle{
    margin-top: 5px;
    color: grey;
    text-align: center
}

.cnter{
    text-align: center
}

.break{
    width: 85%;
    border-top: 1px rgb(168, 166, 166) solid;
    margin-top: 20px;
    height: 50px
}

</style>