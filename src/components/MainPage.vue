<template>
  <div>
    <div class="headPage">
      <div class="titlePage">Current Series</div>
    </div>
    <div class="main">
      <div class="cardcontainer">
        <div v-for="comic in comics" :key="comic.thumb" class="comic">
          <img :src="comic.thumb">
          <h3>{{comic.series}}</h3>
        </div>
      </div>  
    </div>
    <div class="icones">
      <div class="card">
        <img src="@/assets/img/buy-comics-digital-comics.png" alt="">
        <h3>Digital Comics</h3>
      </div>
      <div class="card">
        <img src="@/assets/img/buy-comics-merchandise.png" alt="">
        <h3>DC merchandise</h3>
      </div>
      <div class="card">
        <img src="@/assets/img/buy-comics-subscriptions.png" alt="">
        <h3>Subscription</h3>
      </div>
      <div class="card">
        <img src="@/assets/img/buy-comics-shop-locator.png" alt="">
        <h3>Comic Shop location</h3>
      </div>
      <div class="card">
        <img src="@/assets/img/buy-dc-power-visa.svg" alt="">
        <h3>DC power visa</h3>
      </div>
    </div>
  </div>
</template>

<script>
export default {
 name: 'MainPage',
 data(){
  return{
    comics:[
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
    "price": "$19.99",
    "series": "Action Comics",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
    "price": "$3.99",
    "series": "American Vampire 1976",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
    "price": "$16.99",
    "series": "Aquaman",
    "type": "graphic novel"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
    "price": "$2.99",
    "series": "Batgirl",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    "price": "$3.99",
    "series": "Batman",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    "price": "$2.99",
    "series": "Batman Beyond",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
    "price": "$3.99",
    "series": "Batman/Superman",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
    "price": "$4.99",
    "series": "Batman/Superman Annual",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
    "price": "$5.99",
    "series": "Batman: The Joker War Zone",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
    "price": "$6.99",
    "series": "Batman: Three Jokers",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
    "price": "$4.99",
    "series": "Batman: White Knight Presents: Harley Quinn",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
    "price": "$16.99",
    "series": "Catwoman",
    "type": "graphic novel"
  }
]
  }
 }
}
</script>

<style lang="scss" scoped>
$site_color: #3290FA;
$text_light: white;
*{
  font-weight: 400;
}
.main{
  background: black;
  color: $text_light;
  padding-top: 5rem;
  padding-bottom: 5rem;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
.cardcontainer{
  display: flex;
  flex-wrap: wrap;
  max-width: 1000px;
  gap: .5rem;
  width: 100%;
}

.main h2{
  margin-left: 5rem;
}
.icones{
  padding-top: 5rem;
  padding-bottom: 5rem;
  color: $text_light;
  background: $site_color;
  display: flex;
  align-items: center;
  justify-content: center;
  gap:3rem;
}
.card{
  font-family:Arial, Helvetica, sans-serif!important;
  display: flex;
  align-items: center;
  font-weight: 400;
  gap: 1rem;
  text-transform: uppercase;
  width: calc(100% / 12) * 2;
}
.card img{
  max-width: 100%;
  width: 40px;
} 
.headPage{
  position: relative;
  height: 50vh;
  background-image: url('@/assets/img/jumbotron.jpg');
}
.titlePage{
  padding: 1rem;
  position: absolute;
  bottom: -25px;
  left: 20%;
  background-color: $site_color;
  font-size: 1.5rem;
  text-transform: uppercase;
  color: $text_light;
}
.comic{
  // margin-left: 1rem;
  max-width: calc(((100% / 12) * 4) - .5rem);  
}
.comic h3{
  word-wrap: break-word;
}

</style>