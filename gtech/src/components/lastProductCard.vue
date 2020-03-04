<template>
  <div class="container">
      <div>
            <img class="image" :src="data.url" alt="">
      </div>
      <div class="content">
            <div class="title">
                <h3 class="mr">Porem Ipsum Dolor Sit Ame</h3>
                <p class="mr blur">Consequatur quo voluptatem dolorem</p>
            </div>
            <div>
                <p class="mr">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dolore commodi, fuga doloribus nulla necessitatibus officiis libero, dolorum ut</p>
            </div>
            <div class="wrapButton">
                <button class="button">Read More</button>
                <div>
                    <i class="fas fa-heart icn"></i>
                    <i class="fas fa-comment icn"></i>
                </div>
            </div>
      </div>
  </div>
</template>

<script>
export default {
    props: ['data'],
    created () {
        console.log(this.data)
    }

}
</script>

<style scoped>
.container{
    width: 300px;
    background-color: white!Important;
    margin-left: 20px;
    height: 470px!Important;
    padding-top: 0%!Important
}

.image{
    height: 200px;
    width: 300px
}

.mr{
    margin: 0
}

.content{
    padding-top: 30px;
    padding-left: 20px;
    padding-right: 20px;
    padding-bottom: 20px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    height: 200px;
}

.blur{
    color: rgb(151, 150, 150)
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

.icn{
    color: #EE4F4C;
    font-size: 22px;
    margin-left: 10px;
    margin-right: 10px;
    cursor: pointer;
}

.wrapButton{
    display: flex;
    align-items: center;
    justify-content:space-between;
    margin-top: 10px;
    margin-bottom: 10px
}

</style>