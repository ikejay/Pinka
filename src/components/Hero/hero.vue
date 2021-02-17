<template>
<div id="container">
  <div id="content">
    <div id="texts">
      <h3>The Hero here</h3>
      <p>The main stuffs can be added here</p>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: "hero"
}
</script>

<style scoped>
  #container {
    display: block;
    height: 300px;
  }

  #content {
    height: 300px;
    background: #a7dcd9;
    width: 100%;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  h3{
    font-weight: bold;
    font-size: 60px;
    margin: 0 auto;
    vertical-align: middle;
  }

  #texts {
    position: absolute;
    align-items: center;
    justify-content: center;
    display: block;
  }

  p{
    vertical-align: middle;
  }
</style>