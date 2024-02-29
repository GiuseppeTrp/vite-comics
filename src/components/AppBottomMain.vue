<script>
export default{
    name: "AppBottomMain",
    data() {
    return {
        linksMiddle: [
            {
       title: "DC COMICS",
       links:[
              "Characters",
              "Comics",
              "Movies",
              "TV",
              "Games",
              "Videos",
              "News"
            ]
    },
    {
        title: "DC",
       links:[
              "Terms Of Use",
              "Privacy policy(New)",
              "Ad Choices",
              "Advertising",
              "Jobs",
              "Subscription",
              "Talent Workshops",
               "CPSC Certificates",
               "Rating",
               "Shop Help",
               "Contact Us"

            ]
    },

    {
        title: "SITES",
       links:[
              "DC",
              "MAD Magazine",
              "DC Kids",
              "DC Univere",
              "DC Power Visa"
            ]
    },

    {
        title: "SHOP",
       links:[
              "Shop DC",
              "MAD Magazine",
              
            ]
    },


   
            
        ],

     
  }
 }
}
    </script>

<template>
    <div class="container d-flex flex-wrap flex-row">
        <ul class="list-unstyled text-uppercase">
          <li v-for="(link, index) in linksMiddle" :key="index">
            <a href="" class="text-decoration-none text-dark">
              {{ link.title }}
            </a>
            <ul class="list-unstyled d-flex flex-wrap flex-column"> <!-- Modificata la classe d-flex -->
              <li v-for="(subLink, subIndex) in link.links" :key="subIndex">
                <a href="" class="text-decoration-none text-dark fw-light">
                  {{ subLink }}
                </a>
              </li>
            </ul>
          </li>
        </ul>
      </div>
      
      
      
      
      
      
      
      
      

</template>

<style>

</style>