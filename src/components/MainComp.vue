<template>
    <div>
        <ToolSection/>
        <NetworkSection/>
        <ProjectSection :cards="cards"/>
    </div>
</template>

<script>

import ToolSection from './ToolSection.vue'
import NetworkSection from './NetworkSection.vue'
import ProjectSection from './ProjectSection.vue'

    export default {
        name: 'MainComp',
        components: {
            ToolSection,
            NetworkSection,
            ProjectSection
        },
        props:{
            cards: Array,
        }
    }
</script>

<style lang="scss" scoped>

</style>