<template>
    <div class="container-fluid container-md clients-services-container">


        <h2>Pour les professionnels ET les particuliers</h2>
        <div class="row">
            <div id="proClient" class="col- col-md-6 col-lg-6 pro-client">
                <div class="rounded-and"><p><i class="bi bi-person-plus-fill"></i></p></div>
                <h3>Professionnel</h3>

                <ul class="services-list">
                    <li>Assistance Dépannage informatique</li>
                    <li>Création, Dépannage réseau et internet</li>
                    <li>Cablage de réseau informatique</li>
                    <li>Brassage de baie informatique</li>
                    <li>Installation d'équipements informatiques et d'équipements réseau</li>
                    <li>Mise en service des équipements</li>
                    <li>Récupération des données: disque dur illisible/perte de données</li>
                    <li>Sécurisation de vos données</li>
                    <li>Installation de bornes wifi avec test de couverture ekahau</li>
                    <li>Audit</li>
                </ul>

                <button type="button" class="btn btn-outline-light">Demander un devis</button>

            </div>
            <div id="individualClient" class="col- col-md-6 col-lg-6 individual-client">
                <h3>Particulier</h3>

                <ul class="services-list">
                    <li>Assistance Dépannage informatique</li>
                    <li>Création, Dépannage réseau et internet</li>
                    <li>Cablage de réseau informatique</li>
                    <li>Brassage de baie informatique</li>
                    <li>Installation d'équipements informatiques et d'équipements réseau</li>
                    <li>Mise en service des équipements</li>
                    <li>Récupération des données: disque dur illisible/perte de données</li>
                    <li>Sécurisation de vos données</li>
                    <li>Installation de bornes wifi avec test de couverture ekahau</li>
                    <li>Audit</li>
                </ul>
                <!--

  Assistance dépannage informatique pc-mac à domicile ou en atelier, cours, remise à niveau
  Devis et diagnostique gratuit
  Vente de matériel informatique neuf et reconditionné
Prestation informatique pc de bureau, pc portable :
Besoin d’installer, réinstaller ou faire une migration de votre système d’exploitation Windows, linux, mac os
Remplacement de votre disque dur, mise en place de disque dur SSD
Clonage de votre disque dur
Votre système d’exploitation à planter, votre disque dur est illisible ou vous avez perdu des données
Votre pc est en panne matériel ne s’allume plus ou ne démarre plus (diagnostique gratuit)
Suppression de virus
Récupération de mot de passe perdu
Votre pc rame nettoyage de votre système informatique
Upgrade de votre pc, installation de nouveau périphérique
Optimisation de votre pc
Votre tour pc, pc portable chauffe nettoyage et remplacement de la pâte thermique
Remplacement d’écran, clavier...sur pc portable, pc tout en un
Mise en service de votre matériel informatique
Création de boite mail
 Mise en place de contrôle parental
 Sécurisation de vos données
 Installation de box 
 Installation téléassistance
 Diagnostic des prises téléphoniques et tableau de communication
 Raccordement, création de prise téléphoniques et de tableau de communication
 Test de fonctionnement de votre installation
                -->

            </div>
        </div>
        
    </div>
    
</template>


<script>
export default {
    
}
</script>

<style lang="scss" scoped>
.clients-services-container{
    width: 90%;
    margin: auto;
    .row{
        border: 1px solid #3E83FF;
        border-radius: 15px;
        .pro-client, .individual-client{ padding: 50px;
        @media (max-width: 767px) {
            padding: 50px 30px;
        }}
        .pro-client{  
            background: #3E83FF;
            color: white;
            border-radius: 14px;
            .rounded-and{
                height: 60px;
                width: 60px;
                border-radius: 50%;
                text-align-last: center;
                position: absolute;
                right: -30px;
                top: 50%;
                background: #3E83FF;
                p{
                    margin: none;
                    height: 100%;
                    i{
                        font-size: 35px;
                    }
                }
                @media (max-width: 767px) {
                    top: 94%;
                    right: 135px;
                }
            }

            &:hover{
                box-shadow: inset 0px 0px 10px 1px white;
            }
        }
    }
}
</style>