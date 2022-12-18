<template>
    <div class="container-fluid container-md services-container">
        <h2>Nos prestations</h2>
        <div class="row services">
            <h4>Nous vous proposons une assistance informatique PC/MAC</h4>

            <div class="row pagination-cards">
                <div class="container carousel-container">

                    <input type="radio" name="position" />
                    <input type="radio" name="position" />
                    <input type="radio" name="position" checked />
                    <input type="radio" name="position" />
                    <input type="radio" name="position" />

                    <main id="carousel" class="container">
                        <div class="item">
                            <div class="rounded-bckgrd"><i class="bi bi-pc-display-horizontal"></i></div> 
                            <div class="p"><p>Installation d'équipements informatiques</p></div>   
                        </div>
                        <div class="item">
                            <div class="rounded-bckgrd"><i class="bi bi-clipboard2-pulse"></i></div>
                            <div class="p"><p>Dépannage des équipements informatiques</p></div>
                        </div>
                        <div class="item">
                            <div class="rounded-bckgrd"><i class="bi bi-pc-display"></i></div>
                            <div class="p"><p>Vente de matériel informatique neuf ou reconditionné</p></div>
                        </div>
                        <div class="item">
                            <div class="rounded-bckgrd"><i class="bi bi-hdd-rack"></i></div>
                            <div class="p"><p>Création de réseau internet et Dépannage</p></div>
                        </div>
                        <div class="item">
                            <div class="rounded-bckgrd"><i class="bi bi-keyboard"></i></div>
                            <div class="p"><p>Cours et remise à niveau</p></div>
                        </div>
                    </main>
                  </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Services',
}
</script>

<style lang="scss" scoped>
.carousel-container{
    display: grid
}
#carousel {
  grid-row: 1 / 2;
  grid-column: 1 / 8;
  height: 400px;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  transform-style: preserve-3d;
  perspective: 600px;
  --items: 5;
  --middle: 3;
  --position: 1;
  pointer-events: none;
}

div.item {
    height: 280px;
    display: grid;
    align-content: center;
    border: 1px solid lightgrey;
    border-radius: 15px;
    text-align: center;
  position: absolute;
  width: 300px;
  background: white;
        color: #3E83FF;
    
  --r: calc(var(--position) - var(--offset));
  --abs: max(calc(var(--r) * -1), var(--r));
  transition: all 0.25s linear;
  transform: rotateY(calc(-10deg * var(--r)))
    translateX(calc(-300px * var(--r)));
  z-index: calc((var(--position) - var(--abs)));
  i{font-size: 80px;
   }
  p{
    font-size: 20px;
   }
  
}
div.item:nth-of-type(1) {
  --offset: 1;
}
div.item:nth-of-type(2) {
  --offset: 2;
}
div.item:nth-of-type(3) {
  --offset: 3;
}
div.item:nth-of-type(4) {
  --offset: 4;
}
div.item:nth-of-type(5) {
  --offset: 5;
}

input:nth-of-type(1) {
  grid-column: 2 / 3;
  grid-row: 2 / 3;
}
input:nth-of-type(1):checked ~ main#carousel {
  --position: 1;
}

input:nth-of-type(2) {
  grid-column: 3 / 4;
  grid-row: 2 / 3;
}
input:nth-of-type(2):checked ~ main#carousel {
  --position: 2;
}

input:nth-of-type(3) {
  grid-column: 4 /5;
  grid-row: 2 / 3;
}
input:nth-of-type(3):checked ~ main#carousel {
  --position: 3;
}

input:nth-of-type(4) {
  grid-column: 5 / 6;
  grid-row: 2 / 3;
}
input:nth-of-type(4):checked ~ main#carousel {
  --position: 4;
}

input:nth-of-type(5) {
  grid-column: 6 / 7;
  grid-row: 2 / 3;
}
input:nth-of-type(5):checked ~ main#carousel {
  --position: 5;
}

// .services-container{
//     .pagination-cards{
//         justify-content: center;
//         .cards-grp{
//             height: 350px;
//             justify-content: center;
//             #carouselExampleDark{
//                 height: 100%;
//                 .design-cards{
                    // width: 50%;
                    // display: grid;
                    // align-content: stretch; 
                    // height: 300px;
                    // margin: auto;
                    // border: 1px solid lightgrey;
                    // border-radius: 15px;
                    // text-align: center;
                    // i{font-size: 80px;}
                    // p{font-size: 20px;
                    // color: #485665;}
//                 }
//             nav{
//                 ul{justify-content: center;}
//             }
//             }
//         }
//     }
// }

// .services-container{
//     overflow: hidden;
//     width: 90%;
//     margin: auto;
//     .services{
//         .dts-services{
//         align-items: center;
//         margin: auto;
//         overflow: hidden;
//         .col{
//             display: inline-flex;
//             @media (max-width: 800px){
//                 display: grid;
//                 justify-items: center;
//             }
//         }
        
//         .card-dts{
//             width: 100%;
//             text-align-last: center;
//             align-items: center;
//             .rounded-bckgrd{
//                 width: 80px;
//                 height: 80px;
//                 background: #485665;
//                 border-radius: 50%;
//                 color: white;
//                 i{
//                     font-size: 45px;
//                 }
//             }
//             .p{
//                 margin: auto;
//                 text-align-last: start;
//                 font-size: 20px;
//                 color: #485665;
//                 @media (max-width: 800px) {
//                     font-size: 15px;
//                     text-align: center;
//                     width: 100%;
//                     text-align-last: center; 
//                 }
//             }
//             &:hover{
//             .rounded-bckgrd{
//                 background: #557cb2;
//             }
//             .p{
//                 color: #557cb2;
//             }           
//         }
//         }
//         .card-dts.icons-location{
//             display: grid;
//             .col{
//                 margin: 10px 0;
//             }
//             .house-icon, .shop-icon{
//                 .rounded-bckgrd.house-i, .rounded-bckgrd.shop-i{
//                 width: 60px;
//                 height: 60px;
//                 i{
//                     font-size: 32px;
//                 }
//                 @media (max-width: 800px){
                    
//                     }
//             }
//             p{
//                 font-size: 20px;
//                 align-self: flex-end;
//                 margin-left: 20px;
//                 @media (max-width: 800px){
//                         font-size: 17px;
//                         margin: 0;
//                     }
//             }
//             }
//         }
        
//     }
//     .row-1{
//         transform: translateX(110%);
//         opacity: 0;
//         transition: transform 2s ease-in-out,
//         opacity 0.6s ease-in-out;
//     }
//     .row-1.active{
//         transform: translateX(0%);
//         opacity: 1;
//     }
//     .row-2{
//         transform: translateX(-100%);
//         opacity: 0;
//         transition: transform 2s ease-in-out,
//         opacity 0.6s ease-in-out;
//     }
//     .row-2.active2{
//         transform: translateX(0%);
//         opacity: 1;
//     }
//     }
  
// }

</style>