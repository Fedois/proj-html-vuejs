<script>
import websiteElegant from './websiteElegante.vue'
import learnMore from './learnMore.vue'
import exampleProjects from './exampleProjects.vue'

export default {
    name: 'AppMain',
    components: {
        websiteElegant,
        learnMore,
        exampleProjects
    }
}
</script>

<template>
    <main>
        <websiteElegant />
        <learnMore />
        <exampleProjects />
    </main>
</template>

<style lang="scss" scoped>
section{
    margin: 200px 0;
}
</style>