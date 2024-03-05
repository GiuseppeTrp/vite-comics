<script>
export default {
    name: "AppFooter",

    data() {
        return {
            socials: [
                {
                    name: 'facebook',
                    icon: "/public/img/footer-facebook.png" // Aggiungi l'estensione .png
                },
                {
                    name: 'twitter',
                    icon: "/public/img/footer-twitter.png"
                },
                {
                    name: 'youtube',
                    icon: "/public/img/footer-youtube.png"
                },
                {
                    name: 'pinterest',
                    icon: "/public/img/footer-pinterest.png"
                },
                {
                    name: 'periscope',
                    icon: "/public/img/footer-periscope.png"
                },
            ]
        };
    }
}
</script>

<template>
    <footer class="bg-dark text-white p-5">
      <div class="footer-bottom">
        <div class="container d-flex justify-content-between align-items-center">
          <div class="cta">
            <button class="btn btn-outline-primary text-white p-2 m-3">Sign-up now!</button>
          </div>
          <div class="social-links d-flex gap-2 align-items-center">
            <strong>Follow Us</strong>
            <ul class="list-unstyled d-flex gap-2 mb-0">
              <li v-for="currentSocial in socials" >
                <img :src="currentSocial.icon" :alt="currentSocial.name">
              </li>
            </ul>
          </div>
        </div>
      </div>
    </footer>
  </template>
  
  <style lang="scss">
  .btn {
    padding: 14px 18px;
    text-transform: uppercase;
    font-weight: bold;
    font-size: 1em;
  }
  
  .social-links li {
    list-style: none; 
  }

  
  
  </style>
  
