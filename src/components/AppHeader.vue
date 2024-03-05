<script>
export default{
    name: "AppHeader",

      data() {
        return {
            links: [
                "Characters",
                "Comics",
                "Movies",
                "Tv", 
                "Games",
                "Collectibles",
                "Videos",
                "Fans",
                "News", 
                "Shop"
            ],

           
        }
    }





}




</script>

<template>

    <div class="container-fluid   p-2 header m-3">
        <nav class="text-center d-flex justify-content-around  align-items-center ">
            <div>
                <img  src="/img/dc-logo.png" alt="">

            </div>
            <ul class="d-flex gap-2 list-unstyled text-uppercase align-items-center " >
                <li  v-for="(link, index) in links"
               
            >
                    <a href="" class="text-decoration-none text-dark" >
                    
                        {{ link }}

                    </a>
                </li>
            </ul>

            
            
        </nav>


    </div>

</template>

<style lang="scss">

@use '../styles/header.scss' as *;





 

</style>