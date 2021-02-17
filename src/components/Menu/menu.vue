<template>
  <div id="main">
    <nav id="navi">
      <ul>
        <li><button>Home</button></li>
        <li>Services</li>
        <li>Information</li>
        <li>Products</li>
        <li>Contact Us</li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
name: "menu"
}
</script>

<style scoped>
  #main {
    float: left;
    display: block;
    width: 100%;
  }

 ul {
   display: flex;
   float: right;
 }

 li{
   margin-right: 30px;
   list-style: none;
 }

</style>