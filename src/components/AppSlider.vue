<script>

    export default {
        name: 'AppSlider'
    }

</script>

<template>

    <section>
        <div class="container">
            <div class="title-container">
                <h3>Scopri i prodotti Made in Italy</h3>
                <a href="#">Scopri</a>
            </div>
            <div class="row-slider">
                <div class="category-container">
                    <img src="../assets/img/idee-regalo.jpg" alt="">
                </div>
                <div class="category-container">
                    <img src="../assets/img/cucina.jpg" alt="">
                </div>
                <div class="category-container">
                    <img src="../assets/img/moda.jpg" alt="">
                </div>
                <div class="category-container">
                    <img src="../assets/img/arredamenti.jpg" alt="">
                </div>
                <div class="category-container">
                    <img src="../assets/img/benessere.jpg" alt="">
                </div>
                <div class="category-container">
                    <img src="../assets/img/artigianato.jpg" alt="">
                </div>
                <div class="category-container">
                    <img src="../assets/img/caffetteria.jpg" alt="">
                </div>
            </div>
        </div>
    </section>

</template>

<style scoped lang="scss">
    @use '../style/partials/variables' as *;

    .container {

        background-color: $white;
        padding: 20px;
        display: flex;
        flex-direction: column;
        gap: 20px;

        .title-container{
            display: flex;
            align-items: center;
            gap: 20px;

            a {
                color: $secondary-color;
            }
        }

        .category-container {
            display: flex;
            flex-direction: column;

            img {
                width: 200px;
            }
        }

        .row-slider {
            display: flex;
            gap: 20px;
            overflow-y: scroll;
        }
        

    }

    
    

</style>