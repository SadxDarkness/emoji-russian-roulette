<template>
  <div class="switch">
    <h1 class="switch-title">Choose game mode</h1>
    <div class="switch-buttons">
      <button type="button" class="gradient-button" @click="isDefault = true">
        <span class="gradient-text">Default</span>
      </button>
      <button type="button" class="gradient-button" @click="isDefault = false">
        <span class="gradient-text">Manual</span>
      </button>
    </div>
  </div>
</template>

<script setup>

const props = defineProps({
  modelValue: {
    type: Boolean,
    required: true
  }
})

const emit = defineEmits(['update:modelValue'])
const isDefault = defineModel()

defineOptions({ name: 'SwitchMode' });
</script>

<style lang="scss" scoped src="./style.scss"></style>