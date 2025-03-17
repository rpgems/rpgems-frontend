<script setup lang="ts">
import Card, { CardProps } from './components/Card/Card.vue';

const mockCard: CardProps = {
  title: 'Título',
  cta: {
    label: 'Continuar',
    href: '/continuar',
  },
  iconsList: [
    {
      icon: 'icon',
      label: 'label',
    },
  ],
};

</script>

<template>
  <div class="bg-gradient-to-br from-purple to-purple/80 w-full px-6 pt-6 gap-6 flex flex-col">
    <Card :title="mockCard.title" :cta="mockCard.cta" :iconsList="mockCard.iconsList" />
    <Card :title="mockCard.title" :cta="mockCard.cta" :iconsList="mockCard.iconsList" />
  </div>
</template>