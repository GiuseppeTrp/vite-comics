<script>
export default{
    name: "AppMiddleMain",
   
data() {
  return {
      linksMiddle: [
        {
    image: '../img/buy-comics-digital-comics.png',
    text: "DIGITAL COMICS",
  },
  {
    image: "../img/buy-comics-merchandise.png",
    text: "DC MERCHANDISING",
  },
  {
    image: "../img/buy-comics-digital-comics.png",
    text: "SUBSCRIPTION",
  },
  {
    image: "../img/buy-comics-digital-comics.png",
    text: "COMIC SHOP LOCATOR",
  },
  {
    image: "../img/buy-comics-digital-comics.png",
    text: "DC POWER VISA",
  },
          
      ],

     
  }
}
}
</script>

<template>
    <div class="middle-main container-fluid border">
      <div class="container-fluid">
        <p class="container-fluid text-uppercase p-3">
          <ul class="d-flex gap-5 list-unstyled text-uppercase  justify-content-center ">
            <li class="d-flex gap-2 " v-for="(Middlelink, index) in linksMiddle" :key="index">
              <img :src="Middlelink.image" alt="">
              <a href="" class="text-decoration-none text-light align-self-center">
                {{ Middlelink.text }}
              </a>
            </li>
          </ul>
        </p>
      </div>
    </div>
  </template>
  

<style lang="scss">

@use '../styles/middleMain.scss'  as *;






</style>