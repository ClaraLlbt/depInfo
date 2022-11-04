<template>
    <!--Barre de Navigation-->
    <Navbar />
    <!--Bannière d'en-tête-->
    <HdrBanner />
    
    <Services />

    <Strengths/>
    <!-- <ClientsServices/> -->


</template>


<script>
import HdrBanner from '../components/HdrBanner.vue';
import Navbar from '../components/Navbar.vue';
import Services from '../components/Services.vue';
import Strengths from '../components/Strengths.vue';

export default {
  name: "HomeViewVue",
  components:{
    Navbar,
    HdrBanner,
    Services,
    Strengths
  }
}  
</script>

<style lang="scss">

</style>
