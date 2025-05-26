<template>
    <main>
        <switch-mode  v-model="isDefault"></switch-mode>
        <manual-mode v-if="!isDefault"></manual-mode>
        <default-mode v-else></default-mode>
        <fire-button></fire-button>
    </main>
</template>
<script setup>
import { ref } from 'vue'

import SwitchMode from '@/components/SwitchMode'
import DefaultMode from '@/components/DefaultMode'
import ManualMode from '@/components/ManualMode'
import FireButton from '@/components/FireButton'

defineOptions ({name: 'mainFile'})

const isDefault = ref(true)
</script>

<style lang="scss" scoped src="./style.scss"></style>