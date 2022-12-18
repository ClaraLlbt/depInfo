<template>
<Navbar />
    <div id="contact" class="container-fluid">
        <div class="row row-bnr">
            <HdrBanner  id="HdrBanner" />
        </div>
        <div class="row contact-row">
            <div class="col-10 col-md-3 contact">
                <h1>Contact</h1>
                <div class="col-md- info-contact">
                    <p><i class="bi bi-geo-alt-fill"></i> 813 Avenue Des Moulins
                    83200 - Toulon
                    (sur rendez-vous uniquement)</p>
                    <p><i class="bi bi-phone"></i> 06.27.03.42.16</p>
                    <p><i class="bi bi-at"></i> dito-pro@mail.com</p>
                </div>
                <div class="row networks">
                    <div class="col-6 col-md-3 fb-icon"><i class="bi bi-facebook"></i></div>
                    <div class="col-6 col-md-3 linked-icon"><i class="bi bi-linkedin"></i></div>
                </div>
            </div>
            
                <div class="col-10 col-md-5 forms">
                    <!--Nav Formulaires-->
                    <ul class="nav nav-tabs">
                        <li class="nav-item item-rdv" v-on:click="rdvFormShow()">
                            <a class="nav-link" aria-current="page" href="#form-rdv"> Rendez-vous</a>
                        </li>
                        <li class="nav-item item-devis" v-on:click="devisFormShow()">
                            <a class="nav-link" href="#form-devis"> Devis</a>
                        </li>
                        <li class="nav-item item-info" v-on:click="infoFormShow()">
                            <a class="nav-link" href="#form-info"> Renseignements</a>
                        </li>
                    </ul>

                    <!--Formulaire Devis-->
                    <form id="form-rdv" action="" v-show="rdvForm" class="form-rdv">
                        <label for="" class="txt-label">Vous souhaitez une offre personnalisée sur nos produits ? Remplissez ce formulaire. Nous reviendrons vers vous rapidement avec une offre.</label>
                        <div class="row">
                            <div class="col-md-6">
                            <label for="name">Votre Nom</label>
                            <input arealabel type="text" class="form-control" id="validationTooltip01" required>
                            </div>
                            <div class="col-md-6">
                            <label for="name">Votre prénom</label>
                            <input type="text" class="form-control" id="validationTooltip01" required>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-md-6">
                            <label for="text">Sujet du message</label>
                            <input type="text" class="form-control" id="exampleFormControlInput1" placeholder="">
                            </div>
                            <div class="col-md-6">
                            <label for="number">Téléphone</label>
                            <input type="text" class="form-control" id="exampleFormControlInput1" placeholder="">
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-md">
                                <label for="exampleFormControlTextarea1" class="form-label">Détails de la demande</label>
                                <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
                            </div>
                        </div>
                        <div class="row">
                            <p class="text-muted">*
                                En soumettant ce formulaire, j’accepte que mes informations soient utilisées uniquement dans le cadre de ma demande et de la relation commerciale éthique personnalisée qui peut en découler</p>
                        </div>
                        <div class="row">
                            <button type="button" class="btn btn-primary">Envoyer</button>
                        </div>
                    
                    </form>

                    <!--Formulaire Devis-->
                    <form id="form-devis" action="" v-show="devisForm" class="form-devis">
                        <label for="" class="txt-label">Vous souhaitez une offre personnalisée sur nos produits ? Remplissez ce formulaire. Nous reviendrons vers vous rapidement avec une offre.</label>
                        <div class="row">
                            <div class="col-md-6">
                            <label for="name">Votre Nom</label>
                            <input type="text" class="form-control" id="validationTooltip01" required>
                            </div>
                            <div class="col-md-6">
                            <label for="name">Nom de l'entreprise</label>
                            <input type="text" class="form-control" id="validationTooltip01" required>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-md-6">
                            <label for="email">Votre Email</label>
                            <input type="email" class="form-control" id="exampleFormControlInput1" placeholder="">
                            </div>
                            <div class="col-md-6">
                            <label for="number">Téléphone</label>
                            <input type="text" class="form-control" id="exampleFormControlInput1" placeholder="">
                            </div>
                            
                        </div>
                        <div class="row">
                            <div class="col-">
                            <label for="text">Sujet du message</label>
                            <input type="text" class="form-control" id="exampleFormControlInput1" placeholder="">
                            </div>
                            <div class="col-">
                                <label for="exampleFormControlTextarea1" class="form-label">Détails de la demande</label>
                                <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
                            </div>
                        </div>
                        <div class="row">
                            <p class="text-muted">*
                                En soumettant ce formulaire, j’accepte que mes informations soient utilisées uniquement dans le cadre de ma demande et de la relation commerciale éthique personnalisée qui peut en découler</p>
                        </div>
                        <div class="row">
                            <button type="button" class="btn btn-primary">Envoyer</button>
                        </div>
                    
                    </form>

                    <!--Formulaire Renseignements-->
                    <form id="form-info" action="" v-show="infoForm" class="form-info">
                        <label for="" class="txt-label">Vous souhaitez une offre personnalisée sur nos produits ? Remplissez ce formulaire. Nous reviendrons vers vous rapidement avec une offre.</label>
                        <div class="row">
                            <div class="col-md-6">
                            <label for="name">Votre Nom</label>
                            <input type="text" class="form-control" id="validationTooltip01" required>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-md-6">
                            <label for="name">Nom de la société</label>
                            <input type="text" class="form-control" id="validationTooltip01" required>
                            </div>
                            <div class="col-md-6">
                            <label for="number">Téléphone</label>
                            <input type="number" class="form-control" id="exampleFormControlInput1" placeholder="">
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-md">
                                <label for="exampleFormControlTextarea1" class="form-label">Détails de la demande</label>
                                <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
                            </div>
                        </div>
                        <div class="row">
                            <p class="text-muted">*
                                En soumettant ce formulaire, j’accepte que mes informations soient utilisées uniquement dans le cadre de ma demande et de la relation commerciale éthique personnalisée qui peut en découler</p>
                        </div>
                        <div class="row">
                            <button type="button" class="btn btn-primary">Envoyer</button>
                        </div>
                    
                    </form>
            
            </div>
            
        </div>
    </div>
</template>

<script>
import HdrBanner from '../components/HdrBanner.vue';
import Navbar from '../components/Navbar.vue';


export default {
    name: "contact",
    components: {
        Navbar,
        HdrBanner
    },
    data(){
        return{
            rdvForm : true,
            devisForm: false,
            infoForm: false,
            arrayForms : [],
        }
    },
    mounted(){
        this.displayForm()
    },
    methods: {
        displayForm(){
            const forms = document.querySelectorAll('form')
            for(let i = 0; i < forms.length ; i++){
                this.arrayForms.push(forms[i])
                console.log(this.arrayForms[0]);
            }
            console.log(this.arrayForms);
        },
        rdvFormShow(){
            this.rdvForm =  true
            this.devisForm = false
            this.infoForm = false
        }, 

        devisFormShow(){
            this.rdvForm = false
            this.devisForm = true
            this.infoForm = false
        },
        infoFormShow(){
            this.rdvForm = false
            this.devisForm = false
            this.infoForm = true
        }
    }
}
</script>

<style lang="scss"> 
#HdrBanner{
    h1{ display: none;}
    i{ display: none;}
}
.contact-row{
    justify-content: space-around;
    position: absolute;
    top: 45%;
    .contact{
    background: white;
    height: auto;
    border: 1px solid #3E83FF;
    border-radius: 15px;
    padding: 20px;
    color: #3E83FF;
    @media (max-width: 767px){
        margin-top: 50px;
        padding: 20px;
    }
    h1{
        margin: 20px;
        color: #485665;
        @media (max-width: 767px) {
            font-size: xx-large;
            margin: 10px auto;
        }
    }
    .info-contact{
        p{ margin: 0};
        i{ font-size: 40px}
        @media (max-width: 767px){
            p{
                font-size: 19px;
                font-weight: 600;
                margin-bottom: 10px;
            }
            i{ font-size: 35px;}
        }
    }
    .networks{
        i{ font-size: 30px}
        @media (max-width: 767px){
            text-align: center;
            margin: auto;
            padding: 10px 20px;
            i{ font-size: 40px;}
        }
    }
}
.forms{
    background: white;
    border: 1px solid #3E83FF;
    border-radius: 15px;
    padding: 10px 20px;
    .txt-label{ font-weight: 500;}
    p.text-muted{
        font-size: 12px;
    }
}
@media (max-width: 767px){
    flex-direction: column-reverse;
    align-content: center;
}
}
</style>