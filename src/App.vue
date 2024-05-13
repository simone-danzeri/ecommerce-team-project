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
        <AppFooter></AppFooter>
    </footer>

</template>

<style lang="scss">

    @use './style/generic'; 

</style>
