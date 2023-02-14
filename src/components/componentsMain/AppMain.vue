<script>
import websiteElegant from './websiteElegante.vue'
import learnMore from './learnMore.vue'
import exampleProjects from './exampleProjects.vue'
import phraseClient from './phraseClient.vue'

export default {
    name: 'AppMain',
    components: {
        websiteElegant,
        learnMore,
        exampleProjects,
        phraseClient
    }
}
</script>

<template>
    <main>
        <websiteElegant />
        <learnMore />
        <exampleProjects />
        <phraseClient />
    </main>
</template>

<style lang="scss" scoped>
section{
    margin: 200px 0;
}
</style>