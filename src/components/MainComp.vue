<template>
    <div>
        <ToolSection/>
        <NetworkSection/>
    </div>
</template>

<script>

import ToolSection from './ToolSection.vue'
import NetworkSection from './NetworkSection.vue'

    export default {
        name: 'MainComp',
        components: {
            ToolSection,
            NetworkSection
        }
    }
</script>

<style lang="scss" scoped>

</style>