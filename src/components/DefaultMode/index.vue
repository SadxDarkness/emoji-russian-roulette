<template>
    <img :src="gifs" alt="">
</template>
<script setup>
import setup from './script'

const { gifs } = setup()

defineOptions ({name: 'DefaultMode'})
</script>
<style lang="scss" scoped src="./style.scss"></style>