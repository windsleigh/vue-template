<script setup lang="ts">
import NavbarItem from './components/Navbar/NavbarItem.vue'
import HomeItem from './components/Home/HomeItem.vue'
import AboutItem from './components/About/AboutItem.vue'
import ServicesItem from './components/Services/ServicesItem.vue'
import FooterItem from './components/Footer/FooterItem.vue'
import ContactItem from './components/Contact/ContactItem.vue'
</script>

<template>
  <div class="App">
    <div class="nav"><NavbarItem /></div>
    <div class="rest">
      <HomeItem />
      <AboutItem />
      <ServicesItem />
      <ContactItem />
    </div>
    <div class="footer"><FooterItem /></div>
  </div>
</template>

<style scoped></style>
