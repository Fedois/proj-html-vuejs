<script>
import websiteElegant from './websiteElegante.vue'
import learnMore from './learnMore.vue'
import exampleProjects from './exampleProjects.vue'
import phraseClient from './phraseClient.vue'
import ourBlog from './ourBlog.vue'

export default {
    name: 'AppMain',
    components: {
        websiteElegant,
        learnMore,
        exampleProjects,
        phraseClient,
        ourBlog
    }
}
</script>

<template>
    <main>
        <websiteElegant />
        <learnMore />
        <exampleProjects />
        <phraseClient />
        <ourBlog />
    </main>
</template>

<style lang="scss" scoped>
section{
    margin: 200px 0;
}
</style>