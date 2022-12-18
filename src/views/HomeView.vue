<template>
    <!--Barre de Navigation-->
    <Navbar />
    <!--Bannière d'en-tête-->
    <HdrBanner />
    
    <Services />

    <!-- <Strengths/> -->
    <!-- <ClientsServices/> -->

    <ClientsServices />

    
  <FooterVue />

</template>


<script>
import HdrBanner from '../components/HdrBanner.vue';
import Navbar from '../components/Navbar.vue';
import Services from '../components/Services.vue';
// import Strengths from '../components/Strengths.vue';
import ClientsServices from '../components/ClientsServices.vue';

import FooterVue from '../components/Footer.vue';

export default {
  name: "HomeViewVue",
  components:{
    Navbar,
    HdrBanner,
    Services,
    // Strengths,
    ClientsServices,
    FooterVue,
  }
}  
</script>

<style lang="scss">

</style>
