<template>
  <nav class="navbar bg-white fixed-top">
  <div class="container-fluid">
    <a class="navbar-brand col col-md-6" href="/depInfo/"><img src="../assets/logo-dito.png" alt=""></a>
    <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasNavbar" aria-controls="offcanvasNavbar">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="offcanvas offcanvas-end col col-md-" tabindex="-1" id="offcanvasNavbar" aria-labelledby="offcanvasNavbarLabel">
      <div class="offcanvas-header">
        <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
      </div>
      
      <div class="offcanvas-body">
        <ul class="navbar-nav flex-grow-1 pe-3">
          <li class="nav-item">
            <router-link to="/" style="color:#3E83FF"><i class="bi bi-house-fill"></i> Accueil</router-link>
          </li>
          <li class="nav-item ">
            <a class="nav-link" href="#">Album</a>
          </li>
          <li class="nav-item">
            <router-link to="/contact">Contact</router-link>
          </li>
          <li class="nav-item">
            <div class="btn-group" role="group" aria-label="Basic example">
              <button type="button" class="btn "><a href="#proClient">Professionnel</a></button>
              <button type="button" class="btn "><a href="#individualClient">Particulier</a></button>
            </div>
          </li>
          
        </ul>
      </div>
    </div>
  </div>
</nav>

  
  <!-- <nav class="navbar navbar-expand-lg navbar-light bg-white">
    <div class="container-fluid nav-content">
      <a class="navbar-brand col col-md-6" href="/depInfo/"><p>DiTO-PRO</p></a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      
      <div class="collapse navbar-collapse navbar-list-ul col col-md-"  id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item toDesactivate">
            <a class="nav-link" style="color:#3E83FF" aria-current="page" href="/depInfo/">Accueil</a>
          </li>
          <li class="nav-item activateHomeIcon">
            <a class="nav-link" style="color:#3E83FF"  aria-current="page" href="/depInfo/"><i class="bi bi-house-fill"></i></a>
          </li>
          <li class="nav-item s-toDesactivate">
            <a class="nav-link" href="#">Album</a>
          </li>
          <li class="nav-item s-toDesactivate">
            <a class="nav-link" href="/depInfo/Contact">Contact</a>
          </li>
          <li class="nav-item">
            <div class="btn-group" role="group" aria-label="Basic example">
              <button type="button" class="btn "><a href="#proClient">Professionnel</a></button>
              <button type="button" class="btn "><a href="#individualClient">Particulier</a></button>
            </div>
          </li>
        </ul>
    </div>
  </div>
</nav> -->
</template>

<script>
export default {
  name: "Navbar",  
}
</script>

<style lang="scss">
nav{ box-shadow: 2px 1px 9px grey; }
.navbar-brand{
    color: #3e83ff;
    font-size: 30px;
    padding-left: 15px;
    img{ width: 25%;}
}
#offcanvasNavbar{
  .offcanvas-body{
    ul{
      height: 100%;
      justify-content: space-evenly;
      align-items: center;
      font-size: 20px;
      li.nav-item{
        .btn{
            background: #3e83ff;
            color: white;
            font-weight: bolder;
            &:hover{
              filter: drop-shadow(0px 1px 3px #232323);
            }
            a{
              background-color: none;
              color: white
        }
      }
    }
  }
  }
}



.navbar-toggler{
  @media (min-width: 990px) {
    display: none
 }
}
#offcanvasNavbar{
    @media (min-width: 990px) {
      z-index: 1;
    visibility: initial;
    transform: none;
    border: none;
    position: initial;
    .offcanvas-header{ display: none;}
    .offcanvas-body{
      ul{
        display: inline-flex;
        flex-direction: row;
        width: 100%;
        font-size: 15px;
        li.nav-item{
          margin: auto;
          .btn{
            background: #3e83ff;
            color: white;
            font-weight: bolder;
            &:hover{
              filter: drop-shadow(0px 1px 3px #232323);
            }
            a{
              background-color: none;
              color: white
        }
      }
    }
  }
  }
    }

}

</style>