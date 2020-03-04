<template>
  <div :class="data">
      <div class="left">
          <div>
              <p class="first">Fashion</p>
              <p class="last">Carnival</p>
              <div class="contentSale">
                <p class="infoSale">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
              </div>
              <button class="button">Shop Now</button>
          </div>

      </div>
      <div class="right">

      </div>
  </div>
</template>

<script>
export default {
    props: ['data']

}
</script>

<style>

.left{
    background-color: #D7EFF9;
    width: 100px;
    height: 100%;
    padding-left: 40px;
    display: flex;
    align-items: center
}

.female{
    height: 200px;
    width: 400px;
    background-image: url('https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQLzZIZsqF9xUfRB8dBG2aPmI-MZ31SlTMQshzj4cCjVcRavgYA');
    background-size: cover
}

.male{
    height: 200px;
    width: 400px;
    background-image: url('https://image.shutterstock.com/image-photo/businessman-against-wall-portrait-260nw-575194261.jpg');
    background-size: cover
}

.first{
    font-weight: bold;
    font-size: 30px;
    margin-bottom: 1px;
    margin-top: 0%
}

.last{
    font-weight: bold;
    font-size: 30px;
    margin-bottom: 10px;
    margin-top: 0%;
    color: #EE4F4C
}

.contentSale{
    width: 200px!Important
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

.infoSale{
    color: rgb(71, 68, 68)
}
</style>