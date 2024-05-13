<script>
    export default {
        name: 'AppFooter',
        props: {
            footerKnowLinks: Array,
            footerEarnLinks: Array,
            footerPaymentsLinks: Array,
            footerHelpLinks: Array
        }
    }
</script>

<template>
    <div class="container">
        <div class="ms-footer-top-container d-flex justify-content-around py-4">
            <!-- Conoscersi meglio -->
            <div class="ms-get-to-know-links">
                <ul>
                    <li class="text-white fw-bold">Conoscersi Meglio</li>
                    <li v-for="eachLink in footerKnowLinks" class="py-2">
                        <a class="fw-lighter" href="#">{{eachLink}}</a>
                    </li>
                </ul>
            </div>
            <!-- Guadagna con Amazon -->
            <div class="ms-earn-links">
                <ul>
                    <li class="text-white fw-bold">Guadagna con Amazon</li>
                    <li v-for="eachLink in footerEarnLinks" class="py-2">
                        <a class="fw-lighter" href="#">{{eachLink}}</a>
                    </li>
                </ul>
            </div>
            <!-- Metodi di pagamento -->
            <div class="ms-payments-links">
                <ul>
                    <li class="text-white fw-bold">Metodi di pagamento</li>
                    <li v-for="eachLink in footerPaymentsLinks" class="py-2">
                        <a class="fw-lighter" href="#">{{eachLink}}</a>
                    </li>
                </ul>
            </div>
            <!-- Bisogno di aiuto -->
            <div class="ms-help-links">
                <ul>
                    <li class="text-white fw-bold">Hai bisogno di aiuto?</li>
                    <li v-for="eachLink in footerHelpLinks" class="py-2">
                        <a class="fw-lighter" href="#">{{eachLink}}</a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>


<style scoped lang="scss">
@use '../style/partials/variables' as *;
.ms-footer-top-container{
    background-color: $secondary-color;
    ul{
        list-style: none;
        li{
            list-style: none;
            a{
                text-decoration: none;
                color: #fff;
            }
        }
    }
}
</style>