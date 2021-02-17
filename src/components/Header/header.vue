<template>
<div id="main">
  <div id="container">
    <div id="logoDiv">
      <i class="fa fa-facebook"></i>
    </div>
    <h3>Pinka</h3>
    <Search id="search"></Search>
    <Menu></Menu>
  </div>
</div>

</template>

<script>
import Search from "@/components/Search/search";
import Menu from "@/components/Menu/menu";
export default {
name: "header",
  components: {
              Search,
              Menu
            }
}
</script>

<style scoped>
  #main {
    display: block;
  }
  #container{
    display: flex;
    height: 38px;
    background: cadetblue;
    align-items: center;
  }

  #logoDiv{
    width: 30px;
    height: 30px;
    background-color: slategray;
    margin-right: 20px;
  }

  h3{
    font-family: Monaco;
    margin-right: 20px;
  }

  @media screen and (max-width: 900px){
    #main {

    }

    #search {
      width: 10px;
    }
  }
</style>