<template>
  <div class="container">
    <div class="mainfooter">
      <div class="column">
        <h4>DC Comics</h4>
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
        <h4>Shop</h4>
        <ul>
          <li><a href="#">Shop DC</a></li>
          <li><a href="#">Shop DC Collectibles</a></li>
        </ul>
      </div>
      <div class="column">
        <h4>Dc</h4>
        <ul>
          <li><a href="#">Term of Use</a></li>
          <li><a href="#">Privacy Policy (New)</a></li>
          <li><a href="#">Ad Choices</a></li>
          <li><a href="#">Advertising</a></li>
          <li><a href="#">Jobs</a></li>
          <li><a href="#">Subscriptions</a></li>
          <li><a href="#">Talent Workshops</a></li>
          <li><a href="#">CPSC Certificates</a></li>
          <li><a href="#">Ratings</a></li>
          <li><a href="#">Shop Help</a></li>
          <li><a href="#">Contact US</a></li>
        </ul>
      </div>
      <div class="column">
        <h4>Sites</h4>
        <ul>
          <li><a href="#">DC</a></li>
          <li><a href="#">MAD Magazine</a></li>
          <li><a href="#">DC Kids</a></li>
          <li><a href="#">DC Universe</a></li>
          <li><a href="#">DC Power Visa</a></li>
        </ul>
      </div>
      <div class="image">
        <img src="@/assets/img/dc-logo-bg.png" alt="dc-logo">
      </div>
    </div>
    <div class="socials">
      <button class="btn">SIGN-UP NOW!</button>
      <ul class="follow">FOLLOW US
        <li><a href="#"><i class="fa-brands fa-facebook-f"></i></a></li>
        <li><a href="#"><i class="fa-brands fa-twitter"></i></a></li>
        <li><a href="#"><i class="fa-brands fa-youtube"></i></a></li>
        <li><a href="#"><i class="fa-brands fa-pinterest-p"></i></a></li>
        <li><a href="#"><i class="fa-regular fa-location-pin"></i></a></li>
      </ul>

    </div>
  </div>  
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
$text_light: white;
$text_grayscale: #bdbdbd;
$text_dark: black;
.container{
  background-image: url('@/assets/img/footer-bg.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  color: $text_light;
}
.mainfooter{
  display: flex;
  justify-content: center;
  gap: 1rem;
  margin-left:  calc(100% / 12) * 2;
}
.mainfooter ul{
  list-style: none;
  font-family: Arial, Helvetica, sans-serif !important;
  line-height: 1.4em;
}
.column{
  padding-top: 2rem;
  width: calc(100% / 4) *1;
}
.image{
  width: calc(100% / 4) *3;
}
.mainfooter img{
  max-width: 100%;
  height: 400px;
  object-fit: cover;
}
.mainfooter li a{
  text-decoration: none;
  color: $text_grayscale;
}
.socials{
  background-color: #303030;
  display: flex;
  justify-content: space-around;
  align-items: center;
  padding-top: 1rem;
  padding-bottom: 1rem;
}
.btn{
  background: none;
  border:  2px solid #3290FA;
  padding: 1rem;
  color: $text_light;
}
.btn:hover{
  background-color: white;
  border: 2px solid white;
  color: #303030;
}
.follow{
  list-style: none;
  
}
.follow li {
  display: inline;
  margin-left: 1rem;
  padding: .5rem;
  background-color: white;
  // border-radius: 100% ;
  width: 45px;
  height: 45px;
}

</style>