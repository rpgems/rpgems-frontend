<script setup lang="ts">
import IconInterface from './Icon.interface'
interface VectorIconProps {
  icon: IconInterface;
}
defineProps<VectorIconProps>()

</script>
<template>
    <svg :width="icon.width" :height="icon.height" :viewBox="`0 0 ${icon.width} ${icon.height}`" class="w-[1em] h-auto fill-[currentColor]">
        <path :d="icon.path" />
    </svg>
</template>