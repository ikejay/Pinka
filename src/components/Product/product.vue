<template>
<div id="main">
  <img id="img-div" :src="require(`../../images/blank-image.png`)"/>
  <div id="texts">
    <h2>Product 1</h2>
    <p>Something small about the product</p>
  </div>
  <div id="reviews">
    <img id="rating-image" :src="require(`../../images/5-star-rating.png`)" alt="" />
    <p style="margin-bottom: 25px;">Reviews</p>
  </div>
  <div id="price">
    <h3 style="font-family: Monaco; text-align: right; font-weight: bold; font-size: 20px">GH¢25</h3>
  </div>
  <hr style="width: 96%; position: relative; text-align: center; margin: auto; border: none; height: 1px; background-color: lightgrey" />
  <h3></h3>
  <div id="butts">
    <button style="background-color: darkcyan; width: 120px; height: 35px">Add to cart</button>
    <button style='width: 35px; height: 30px; margin-left: 10px; background-color: white; border: lightgrey solid 1px; background-image: url("../../images/")'></button>
  </div>
  <div style="margin-right: 100px; background-color: #a7dcd9; align-items: center; width: 100%">
    <select style="float: right">
      <option>1</option>
    </select>
  </div>
</div>
</template>

<script>
export default {
name: "product",

  data() {
    return{
      imag: ""
    }
  }
}

</script>

<style scoped>

#main {
  width: 500px;
  border: lightgrey solid 1px;
  height: 600px;
  margin: 20px;
  border-radius: 5px;
  cursor: pointer;
}

#img-div {
  margin-top: 10px;
  height: 350px;
  width: 480px;
  border-radius: 5px;
  border: none;
}

#texts{
  width: 480px;
  height: 70px;
  position: relative;
  margin: 0 auto;
}

h2{
  text-align: left;
}

p{
  text-align: left;
}

#rating {
  width: 250px;
  height: 300px;
}

#reviews{
  width: 100px;
  margin: 0 auto;
  float: left;
  padding-left: 10px;
  filter: opacity(0.5) drop-shadow(0 0 0 lightgrey);
}

#price{
  margin: 10px;
  color: gray;
}

#reviews p{
  font-family: Monaco;
  font-weight: bold;
}

#rating-image{
  width: 100px;
  height: 20px;
}

#butts{
  clear: both;
  margin-top: 20px;
  justify-content: left;
  float: left;
  margin-left: 2%;
  height: 35px;
  display: flex;
  align-items: center;
}

button{
  border-radius: 5px;
  font-family: Monaco;
  border: none;
  color: white;
}
</style>