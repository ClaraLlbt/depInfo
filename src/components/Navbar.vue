<template>
  <nav class="navbar navbar-expand-lg bg-white">
    <div class="container-fluid nav-content">
      <a class="navbar-brand col" href="#"><p>DEPANNAGE INFORMATIQUE</p></a>
      <div class="navbar-list-ul col" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item toDesactivate">
            <a class="nav-link" style="color:#3E83FF" aria-current="page" href="#">Accueil</a>
          </li>
          <li class="nav-item activateHomeIcon">
            <a class="nav-link" style="color:#3E83FF"  aria-current="page" href="#"><i class="bi bi-house-fill"></i></a>
          </li>
          <li class="nav-item toDesactivate">
            <a class="nav-link" href="#">Album</a>
          </li>
          <li class="nav-item toDesactivate">
            <a class="nav-link" href="#">Qui sommes-nous?</a>
          </li>
          <li class="nav-item">
            <div class="btn-group" role="group" aria-label="Basic example">
              <button type="button" class="btn ">Professionnel</button>
              <button type="button" class="btn ">Paticulier</button>
            </div>
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
    .navbar-list-ul{
      ul{
        width: 100%;
        justify-content: flex-end;
        justify-content: space-between;
        .activateHomeIcon{
          display: none;
        }
        li{
          .btn{
            background: #3e83ff;
            color: white;
            font-weight: bolder;
            &:hover{
              filter: drop-shadow(0px 1px 3px #232323);
            }
          }
        }
      }
      @media (max-width: 990px) {
        ul{
          display: inline-flex;
          flex-direction: row;
          justify-content: space-between;
          li.toDesactivate{
            display: none;
          }
          li.activateHomeIcon{
            display: block;
          }
        }
      }

    }
  }
}
</style>