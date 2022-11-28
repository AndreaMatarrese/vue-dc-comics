<template>
   <div>
      <div class="container-fluid">
         <div class="lm row">
               <img src="@/assets/img/dc-logo.png" alt="dclogo">
               <ul>
                  <li><a href="http://localhost:8080/#">Characters</a></li>
                  <li><a href="#">Comics</a></li>
                  <li><a href="#">Movies</a></li>
                  <li><a href="#">Tv</a></li>
                  <li><a href="#">Games</a></li>
                  <li><a href="#">Collectibles</a></li>
                  <li><a href="#">Videos</a></li>
                  <li><a href="#">Fans</a></li>
                  <li><a href="#">News</a></li>
                  <li><a href="#">Shop</a></li>
               </ul>
         </div>
      </div>
   </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
$row_display: flex;

img{
   max-width: 100%;
}
  .row{
   display: $row_display;
  }
.lm{
   display: flex;
   justify-content: space-around;
   align-items: center;
}
  ul{
   list-style: none;
   display: flex;
   gap: 1rem;
   font-weight: 400;
   text-transform: uppercase;
  }

  li a{
   color: black;
   text-decoration: none;
   padding-top: 2.5rem;
   padding-bottom: 2.5rem;
  }
  li a:focus{
   color: #3290FA;
   border-bottom: 4px solid #3290FA;
   
  }
   
</style>