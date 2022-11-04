<template>
  <nav class="navbar navbar-expand-lg bg-white">
    <div class="container-fluid nav-content">
      <a class="navbar-brand" href="#">DEPANNAGE INFORMATIQUE - Toulon-Ouest</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Accueil</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Album</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Qui sommes-nous?</a>
          </li>

          <li class="nav-item">
            <a class="nav-link" href="#">Particulier</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Professionnel</a>
          </li>
      
        </ul>
    </div>
  </div>
</nav>
</template>


<script>
export default {
  name: "Navbar"
  
}
</script>

<style lang="scss" scoped>
.navbar{
  position: fixed;
  z-index: 1;
  width: 100%;
  top: 0;
  .nav-content{
    .navbar-brand{
      color: #3E83FF
    }
    .navbar-collapse{
      ul{
        width: 100%;
        justify-content: flex-end;
      }
    }
  }
}
</style>