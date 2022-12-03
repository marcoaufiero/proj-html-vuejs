<template>
    <div>
        <ToolSection/>
        <NetworkSection/>
        <ProjectSection :cards="cards"/>
        <ManagementSection/>
        <TestimonialSection/>
    </div>
</template>

<script>

import ToolSection from './ToolSection.vue'
import NetworkSection from './NetworkSection.vue'
import ProjectSection from './ProjectSection.vue'
import ManagementSection from './ManagementSection.vue'
import TestimonialSection from './TestimonialSection.vue'

    export default {
        name: 'MainComp',
        components: {
            ToolSection,
            NetworkSection,
            ProjectSection,
            ManagementSection,
            TestimonialSection
        },
        props:{
            cards: Array,
        }
    }
</script>

<style lang="scss" scoped>

</style>