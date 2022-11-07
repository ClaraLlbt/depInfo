<template>
    <div class="container-fluid container-md services-container">
        <h2>Nos prestations</h2>
        <div class="row services">
            <h4>Nous vous proposons une assistance informatique PC/MAC</h4>

            <div class="row dts-services row-1">

                <div class="col card-dts icons-location">
                    <div class="col house-icon">
                        <div class="rounded-bckgrd house-i"><i class="bi bi-house-door"></i></div>
                        <p class="p">Site Client</p>
                    </div>
                    <div class="col shop-icon">
                        <div class="rounded-bckgrd shop-i"><i class="bi bi-shop"></i></div>
                        <p class="p">A l'atelier</p>
                    </div>
                </div>
                <div class="col card-dts">
                    <div class="col-4 rounded-bckgrd"><i class="bi bi-pc-display-horizontal"></i></div> 
                    <div class="col-8 p"><p>Installation d'équipements informatiques</p></div>
                </div>
                <div class="col card-dts">
                    <div class="col-4 rounded-bckgrd"><i class="bi bi-clipboard2-pulse"></i></div>
                    <div class="col-8 p"><p>Dépannage des équipements informatiques</p></div>
                </div>
            </div>
            
            <div class="row dts-services row-2">
                <div class="col card-dts">
                    <div class="col-4 rounded-bckgrd"><i class="bi bi-pc-display"></i></div>
                    <div class="col-8 p"><p>Vente de matériel informatique neuf ou reconditionné</p></div>
                </div>
                <div class="col card-dts">
                    <div class="col-4 rounded-bckgrd"><i class="bi bi-hdd-rack"></i></div>
                    <div class="col-8 p">Création de réseau internet et Dépannage</div>
                </div>
                <div class="col card-dts">
                    <div class="col-4 rounded-bckgrd"><i class="bi bi-keyboard"></i></div>
                    <div class="col-8 p"><p>Cours et remise à niveau</p></div>
                    
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Services',
    mounted(){
        this.displayContainer()
    },
    methods:{
        displayContainer(){
            const servicesBloc = document.querySelector('.services-container');
            const row1 = document.querySelector('.row-1')
            const row2 = document.querySelector('.row-2')
            
            window.addEventListener('scroll', () => { 
        const { scrollTop, scrollHeight ,clientHeight} = document.documentElement;
        const topElementToTopViewport = servicesBloc.getBoundingClientRect().top
        if(scrollTop > (scrollTop + topElementToTopViewport).toFixed() - clientHeight * 0.30){
          row1.classList.add('active');
          row2.classList.add('active2')
        }
      });
        }
    }
}
</script>

<style lang="scss" scoped>
.services-container{
    overflow: hidden;
    width: 90%;
    margin: auto;
    h2{
        margin: 50px 0;
    }
    .services{
        .dts-services{
        align-items: center;
        margin: auto;
        overflow: hidden;
        .col{
            display: inline-flex;
            @media (max-width: 800px){
                display: grid;
                justify-items: center;
            }
        }
        
        .card-dts{
            width: 100%;
            text-align-last: center;
            align-items: center;
            .rounded-bckgrd{
                width: 80px;
                height: 80px;
                background: #485665;
                border-radius: 50%;
                color: white;
                i{
                    font-size: 45px;
                }
            }
            .p{
                margin: auto;
                text-align-last: start;
                font-size: 20px;
                color: #485665;
                @media (max-width: 800px) {
                    font-size: 15px;
                    text-align: center;
                    width: 100%;
                    text-align-last: center; 
                }
            }
            &:hover{
            .rounded-bckgrd{
                background: #557cb2;
            }
            .p{
                color: #557cb2;
            }           
        }
        }
        .card-dts.icons-location{
            display: grid;
            .col{
                margin: 10px 0;
            }
            .house-icon, .shop-icon{
                .rounded-bckgrd.house-i, .rounded-bckgrd.shop-i{
                width: 60px;
                height: 60px;
                i{
                    font-size: 32px;
                }
                @media (max-width: 800px){
                    
                    }
            }
            p{
                font-size: 20px;
                align-self: flex-end;
                margin-left: 20px;
                @media (max-width: 800px){
                        font-size: 17px;
                        margin: 0;
                    }
            }
            }
        }
        
    }
    .row-1{
        transform: translateX(110%);
        opacity: 0;
        transition: transform 2s ease-in-out,
        opacity 0.6s ease-in-out;
    }
    .row-1.active{
        transform: translateX(0%);
        opacity: 1;
    }
    .row-2{
        transform: translateX(-100%);
        opacity: 0;
        transition: transform 2s ease-in-out,
        opacity 0.6s ease-in-out;
    }
    .row-2.active2{
        transform: translateX(0%);
        opacity: 1;
    }
    }
  
}

</style>