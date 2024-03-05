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
  <div class="container-fluid d-flex flex-wrap flex-row gap-2 flex-wrap text-white justify-content-center" id="background">
    
    <div v-for="currentLinkList in linksMiddle" class="  d-flex flex-column text-center  py-5" >
        <h4 class="title-link">{{ currentLinkList.title }}</h4>
        <ul class="list-unstyled ">
            <li class="links-bottom" v-for="currentLink in currentLinkList.links" >{{ currentLink }}</li>
            
        </ul>
    </div>
    
          

    
    
</div>

      
      
      
      
      
      
      
      

</template>

<style lang="scss">
.links-bottom{
  font-size: 10px;
}

.title-link{
  font-size: 15px
}

#background{
  background-image: url('../img/footer-bg.jpg');
  background-position: center;
  background-repeat: no-repeat;
  
}

#content {
  background-image: url('../img/dc-logo-bg.png');
  background-repeat: no-repeat;
  background-position: center;
  width: 700px ;
  height: 400px;
  
  
  
  
  
}




</style>