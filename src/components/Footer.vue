<template>
    <footer class="container-fluid">
        <div class="container-lg">
            <div class="row">
                <div class="col-lg-4 about-blc">
                    <h3>A propos</h3>
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Facilis eos necessitatibus dignissimos velit dicta vero labore. Vero porro eos, deleniti ipsum id iure? Ipsa dignissimos laborum consequuntur sunt corrupti nam!</p>
                </div>
                <div class="col-lg-4 contact-blc">
                    <h3>Nous contacter</h3>

                    <div class="row">
                        <div class="col-lg-2 phone-icon"><i class="bi bi-phone"></i></div>
                        <div class="col-lg-10 phone-nb"><p>06.27.03.42.16</p></div>
                    </div>
                    <div class="row">
                        <div class="col-lg-2 mail-icon"><i class="bi bi-at"></i></div>
                        <div class="col-lg-10 mail-adress"><p>dito-pro@mail.com</p></div>
                    </div>
                </div>
                <div class="col-lg-4">
                    <h3>Zone d'intervention</h3>
                    <P>83 - Var</P>
                    <p>06 - Alpes Maritimes</p>
                    <p>13 - Bouche-du-Rhône</p>
                </div>
            </div>

        </div>
    </footer>
</template>

<script setup lang="ts">

</script>

<style lang="scss" scoped>
.container-fluid{
    color: white;
    margin-top: 50px;
    padding-top: 50px;
    background: #3e83ff;
    .about-blc{
        p{
            width: 85%;
            text-align: justify;
        }
    }
    .contact-blc{
        .row{
            font-size: 20px;
        }
    }
}

</style>