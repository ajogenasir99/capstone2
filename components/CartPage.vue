<template>

    <div class="cart">
         <div class="header">
            <router-link to="/"><h1>Shopping Website.</h1></router-link>
            <img src="./assets/cartCheck.png">
        </div>
        <div class="main">
          
          <div class="title">
            <p>Product</p>
            <p>Description</p>
            <p>Quantity</p>
            <p>Price</p>
            <p>Remove</p>
          </div>
          <hr>
          <div class="product">
            <img src="./assets/Dsneaks1.png" alt="sneakers selection">
            <p id="desc">Lorem</p>
            <p id="quantity">5</p>
            <p id="price">N25</p>
            <p id="remove">x</p>
          </div>

          <div class="product">
            <img src="./assets/Dsneaks3.png" alt="sneakers selection">
            <p id="desc">Lorem</p>
            <p id="quantity">1</p>
            <p id="price">N25</p>
            <p id="remove">x</p>
          </div>
          <hr>
        <p id="total">Total: N150</p>
        </div>
      </div>
    

</template>

<script>
export default {

}
</script>

<style scoped>
*{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}
.header{
  width:90%;
  margin:0 auto;
  height: 10vh;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.header h1{
  font-size: 20px;
}
.header a{
    text-decoration: none;
    color: black;
}
.header img{
  width: 30px;
  height: 30px;
  cursor: pointer;
}



.cart .main{
  width: 80%;
  margin: 0 auto;
  padding: 20px 0;
}

.cart .main .title{
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  place-content: center;
  padding-bottom:10px;
}

.cart .main .title p{
  width: 100%;
}

.cart .main #total{
  text-align: right;
  padding-top: 20px;
  font-size: 50px;
}

.cart .main .product{
  padding: 20px 0;
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  place-items: center;
}

.cart .main .product #remove{
  font-weight: bolder;
  cursor: pointer;
}

.cart .main .product p{
  width: 100%;
}

.cart .main .product img{
  width: 100%;
  height: 200px;
}

</style>