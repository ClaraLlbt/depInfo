<template>
    <!--Barre de Navigation-->
    <Navbar />
    <!--Bannière d'en-tête-->
    <HdrBanner />
    
    <Services />


</template>


<script>
import HdrBanner from '../components/HdrBanner.vue';
import Navbar from '../components/Navbar.vue';
import Services from '../components/Services.vue';

export default {
  name: "HomeViewVue",
  components:{
    Navbar,
    HdrBanner,
    Services
  }
}  
</script>

<style lang="scss">

</style>
