<script>
    export default {
        name: 'AppHeader'
    }
</script>

<template>


    <section class="d-flex justify-content-between align-items-center p-2">
        
        <!--LOGO-->
        <div>
            <img src="" alt="">LOGO
        </div>

        <!--NAME USER & LOCATION-->
        <div class="d-flex">
            <div><i>X</i></div>

            <div>
                <div>Invia a Mattia</div>
                <div>Valenzano 70010</div>
            </div>
        </div>


        <!--SEARCHBAR-->
        <div class="d-flex">

            <div>tutte le categorie</div>

            <form class="d-flex" role="search">
             <input class="form-control me-2" type="search" placeholder="Ricerca Amazon.it" aria-label="Search">
            </form>
            
            
            <div></div>
            <div>X</div>
        </div>

        <!--ACCOUNT & LISTS-->
        <div>
            <div>Ciao Mattia</div>
            <div>Account e liste</div>
            <i></i>
        </div>

        <!--ORDERS-->
        <div>
            <div>Resi</div>
            <div>E ordini</div> 
        </div>

        <!--CART-->
        <div>
            <i></i>
            <span>0</span>
            <div>Carrello</div> 
        </div>
        
    </section>
    
</template>


<style scoped lang="scss">
@use '../style/partials/variables' as *;
</style>