<template>
  <div class="footer">
    <!-- Footer content -->
    <div class="footerPadding">
      <!-- Top section -->
      <div class="footerTop">
        <!-- Logo -->
        <h2 class="footerLogo">Site</h2>
        <!-- Links -->
        <div class="footerLinks">
          <!-- Contact info -->
          <div class="footerLinksDiv">
            <h4>Contact Us</h4>
            <p>contact@site.com</p>
          </div>
          <!-- Social media links -->
          <div class="footerLinksDiv">
            <h4>Connect</h4>
            <div class="socialmedia">
              <a href="https://www.instagram.com/">
                <i class="fab fa-instagram icon"></i>
                Instagram
              </a>

              <a href="https://www.linkedin.com/">
                <i class="fab fa-linkedin icon"></i>
                LinkedIn
              </a>
              <a href="">
                <i class="fab fa-whatsapp icon"></i>
                +56 9 1234 5678
              </a>
            </div>
          </div>
        </div>
      </div>
      <!-- Bottom section -->
      <hr />
      <div class="footerBelow">
        <div class="footerCopyright">
          <!-- Copyright info -->
          <p>@{{ currentYear }} Site - All rights reserved</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const currentYear = ref(new Date().getFullYear())
</script>

<style scoped>
.footer {
  color: rgb(0, 0, 0);
  bottom: 0;
  width: 100%;
  background: rgb(255, 255, 255);
  opacity: 1;
  font-size: 1.5rem;
  border: 5px solid rgb(3, 3, 3);
}

.footerPadding {
  padding: 2rem;
  display: flex;
  flex-direction: column;
}

.footerLinks {
  display: flex;
  justify-content: space-around;
  align-items: flex-start;
  flex-wrap: wrap;
  width: 100%;
  text-align: left;
  margin-bottom: 2rem;
}

.footerLinksDiv {
  display: flex;
  align-items: flex-start;
  flex-direction: column;
  flex-wrap: wrap;
  width: 250px;
  text-align: left;
}

a {
  text-decoration: none;
  color: rgb(0, 0, 0);
  padding: 10px;
}

.socialmedia a {
  display: flex;
  align-items: center;
}

.socialmedia span {
  margin-left: 10px;
}

.socialmedia .icon {
  margin-right: 10px;
}

.footerBelow {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 5px;
  margin-top: 2rem;
}

hr {
  color: rgb(0, 0, 0);
  width: 90%;
  margin-top: 1rem;
}

.footerBelow p {
  font-size: 13px;
  line-height: 15px;
  color: rgb(0, 0, 0);
  font-weight: 600;
  padding-bottom: 5px;
}

.footerTop {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-bottom: 5px;
}

.footerLogo {
  margin-bottom: 1rem;
  font-size: 24px;
  font-weight: bold;
}

@media (max-width: 482px) {
  .footerLinks {
    flex-direction: column;
    align-items: center;
  }

  .footerLinksDiv {
    width: 100%;
    margin-bottom: 1rem;
    align-items: center;
  }

  .socialmedia a {
    margin-bottom: 5px;
  }
}
.icon {
  margin-right: 10px;
}
</style>
