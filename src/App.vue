<script>

import AppSlider from './components/AppSlider.vue'
import AppHeader from './components/AppHeader.vue'
import AppFooter from './components/AppFooter.vue'; 

export default {
    components: {
        AppHeader,
        AppSlider,
        AppFooter
    },
    data () {
        return {
            footerKnowLinks: [
                'Opportunità di lavoro',
                'Informazioni su Amazon',
                'Sostenibilità',
                'Amazon Science'
            ],
            footerEarnLinks: [
                'Vendi su Amazon',
                'Vendi su Amazon Business',
                'Vendi prodotti innovativi',
                'Costruisci e proteggi il tuo marchio',
                'Diventa affiliato',
                'Lavora con noi',
                'Amazon Pay'
            ],
            footerPaymentsLinks: [
                'Metodi di pagamento',
                'Convertitore di valuta Amazon',
                'Buoni regalo',
                'Ricarica online'
            ],
            footerHelpLinks: [
                'Visualizza o traccia un ordine',
                'Costi e modalità di spedizione',
                'Amazon Prime',
                'Restituisci un ordine',
                'Servizio Clienti'
            ]
        }
    }
}

</script>

<template>

    <header>
        <AppHeader></AppHeader>
    </header>

    <main>
        <AppSlider></AppSlider>
    </main>

    <footer>
        <AppFooter :footerKnowLinks="footerKnowLinks" :footerEarnLinks="footerEarnLinks" :footerPaymentsLinks="footerPaymentsLinks" :footerHelpLinks="footerHelpLinks"></AppFooter>
    </footer>

</template>

<style lang="scss">

    @use './style/generic'; 

</style>
