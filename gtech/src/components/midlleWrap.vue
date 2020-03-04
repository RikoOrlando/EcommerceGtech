<template>
  <div class="container">
      <div class="box">
          <div class="top">
              <div class="wrapIconTop">
                  <div class="wrapIcon">
                      <div class="iconTop">
                          <i class="fas fa-truck sizeIcon"></i>
                      </div>
                      <div>
                          <h2 class="resetMargin">Free Shipping</h2>
                          <p class="resetMargin childFitur">With $50 or more orders</p>
                      </div>
                  </div>
                  <div class="wrapIcon">
                      <div class="iconTop">
                          <i class="fas fa-dollar-sign sizeIcon"></i>
                      </div>
                      <div>
                          <h2 class="resetMargin">Free Refund</h2>
                          <p class="resetMargin childFitur">100% Refund Within 3 days</p>
                      </div>
                  </div>
                  <div class="wrapIcon">
                      <div class="iconTop">
                          <i class="fas fa-headset sizeIcon"></i>
                      </div>
                      <div>
                          <h2 class="resetMargin">Support 24.7</h2>
                          <p class="resetMargin childFitur">call us anytime you want</p>
                      </div>
                  </div>
              </div>
          </div>
          <div class="center">
                <div class="wrapCarnival">
                    <bannerSale :data="'female'"></bannerSale>
                    <bannerSale :data="'male'"></bannerSale>
                </div>
                <sale></sale>
          </div>
      </div>
  </div>
</template>

<script>
import sale from './saleWrap'
import bannerSale from './saleBanner'
export default {
    components: {sale, bannerSale},
    data () {

    }
}
</script>

<style scoped>
.container{
    height: 800px;
    display: flex;
    justify-content: center;
    align-items: center;
    background: url('https://www.rapormerah.co/wp-content/uploads/2017/08/geometic-bg-white-3.jpg');
    flex-wrap: wrap
}
.box{
    height: 110%;
    width: 65%;
    background-color: white;
    z-index: 2;
}

.center{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100%;
    flex-direction: column;
    flex-wrap: wrap

}
.wrapCarnival{
    display: flex;
    justify-content: space-around;
    width: 80%;
    margin-bottom: 50px;
    padding-left: 90px;
    padding-right: 90px
}
.top{
    display: flex;
    width: 100%;
    justify-content: center;
    margin-top: -50px;
}

.wrapIcon{
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center
}

.iconTop{
    border: 1px solid white;
    height: 100px;
    width: 100px;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 50%;
    background-color: white
}

.sizeIcon{
    font-size: 40px
}

.resetMargin{
    margin: 0%
}

.wrapIconTop{
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
    width: 100%
}

.childFitur{
    color: grey;
    margin-top: 5px
}

</style>