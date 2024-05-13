<script>

import AppSlider from './components/AppSlider.vue'
import AppHeader from './components/AppHeader.vue'

export default {
    components: {
        AppHeader,
        AppSlider
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

</template>

<style lang="scss">

    @use './style/generic'; 

</style>
