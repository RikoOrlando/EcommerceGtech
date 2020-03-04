<template>
  <div class="footContainer">
      <div class="sizeBox">
        <h3>About Company</h3>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. In beatae unde quas mollitia itaque minus</p>
      </div>
      <div class="sizeBox">
        <h3>My Account</h3>
        <p class="mtBreak">My Account</p>
        <p class="mtBreak">Contact</p>
        <p class="mtBreak">Checkout</p>  
      </div>
      <div class="sizeBox">
        <h3>Product</h3>
        <p class="mtBreak">About Us</p>
        <p class="mtBreak">Blog</p>
        <p class="mtBreak">Contact</p>
        <p class="mtBreak">Services</p>
      </div>
      <div class="sizeBox">
        <div>
          <h3>Follow Us</h3>
          <p class="mtBreak"><i class="fab fa-google"></i> Google</p>
          <p class="mtBreak"><i class="fab fa-facebook"></i> Facebook</p>
          <p class="mtBreak"><i class="fab fa-twitter"></i> Twitter</p>
        </div>
        <div>
          <h3>Payment Method</h3>
          <div class="paymentWrap">
            <i class="fas fa-credit-card"></i>
            <i class="fab fa-cc-amazon-pay"></i>
            <i class="fab fa-cc-mastercard"></i>
            <i class="fab fa-cc-visa"></i>
          </div>
        </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>

.footContainer{
    height: 280px;
    background: rgb(0,0,0);
    background: linear-gradient(90deg, rgba(0,0,0,1) 0%, rgba(237,86,24,1) 0%, rgba(255,105,132,1) 100%, rgba(0,0,0,1) 100%);
    display: flex;
    justify-content: center;
    padding-top: 50px;
    color: whitesmoke;
    font-family: Verdana, Geneva, Tahoma, sans-serif
}

.sizeBox{
  width: 15%;
  margin: 10px
}

.mtBreak{
  margin-bottom: 1px;
  margin-top: 1px;
  cursor: pointer;
}

.paymentWrap{
  display: flex;
  flex-direction: row;
  width: 55%;
  justify-content:space-between
}

</style>