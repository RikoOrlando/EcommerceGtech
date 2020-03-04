<template>
  <div class="containerWrap font">
    <div class="nav fontStyleNav">
      <div class="containerNav">
          <div>
              <h1>Gtech Store</h1>
          </div>
          <div class="navRight">
              <h4 class="breakMT">Home</h4>
              <h4 class="breakMT">Shop</h4>
              <h4 class="breakMT">Products</h4>
              <h4 class="breakMT">Cart</h4>
              <h4 class="breakMT">Account</h4>
          </div>
      </div>
    </div>
    <banner></banner>
    <middle></middle>
    <lastestProduct></lastestProduct>
    <favourite></favourite>
    <logo></logo>
    <footerC></footerC>
  </div>
</template>

<script>
import banner from '../components/banner'
import middle from '../components/midlleWrap'
import lastestProduct from '../components/lastestProduct'
import favourite from '../components/favourite'
import logo from '../components/logoWrap'
import footerC from '../components/footer'
export default {
  components: {banner, middle, lastestProduct, favourite, logo, footerC}
}
</script>

<style scoped>
.nav{
  height: 50px;
  background-color: #EE4F4C;
  align-items: center;
  display: flex;
  justify-content: center
}

.containerNav{
  width: 65%;
  display: flex;
  justify-content:space-between;
  align-items: center
}

.fontStyleNav{
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  color: whitesmoke
}

.font{
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}

.navRight{
  display: flex;
  height: 100%;
  justify-content:space-around;
  width: 50%
}

.breakMT{
  cursor: pointer;
}

</style>