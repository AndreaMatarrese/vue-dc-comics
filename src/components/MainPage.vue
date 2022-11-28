<template>
  <div>
    <div class="main">
      <H2>--- Content Goes here --- </H2>
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

}
</script>

<style lang="scss" scoped>
$text_light: white;
*{
  font-weight: 400;
}
.main{
  background: black;
  color: $text_light;
  padding-top: 5rem;
  padding-bottom: 5rem;
}

.main h2{
  margin-left: 5rem;
}
.icones{
  padding-top: 5rem;
  padding-bottom: 5rem;
  color: $text_light;
  background: #3290FA;
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
}
.card img{
  max-width: 100%;
  width: 40px;
} 
</style>