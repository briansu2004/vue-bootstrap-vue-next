<template>
  <component :is="tag" class="row d-flex flex-wrap">
    <slot />
  </component>
</template>

<script setup lang="ts">
interface BFormRowProps {
  tag?: string
}

withDefaults(defineProps<BFormRowProps>(), {
  tag: 'div',
})
</script>
