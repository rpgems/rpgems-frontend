<script lang="ts" setup>
interface CardProps {
  title: string;
  cta: {
    label: string;
    href: string;
  };
  iconsList: {
    icon: string;
    label: string;
  }[];
}

const props: CardProps = defineProps<{
    title: string;
    cta: {
        label: string;
        href: string;
    };
    iconsList: {
        icon: string;
        label: string;
    }[];
}>();
</script>

<template>
    <div
        class="bg-rpg-background/40 p-4 rounded-lg border border-rpg-accent/20 hover:border-rpg-accent/40 transition-colors animate-fade-in">
        <h3 class="text-lg font-semibold text-rpg-text mb-2">{{ title }}</h3>
        <div class="flex items-center space-x-4 text-rpg-text/60 mb-4">
            <div class="flex items-center space-x-1">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor"
                    stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-users h-4 w-4">
                    <path d="M16 21v-2a4 4 0 0 0-4-4H6a4 4 0 0 0-4 4v2"></path>
                    <circle cx="9" cy="7" r="4"></circle>
                    <path d="M22 21v-2a4 4 0 0 0-3-3.87"></path>
                    <path d="M16 3.13a4 4 0 0 1 0 7.75"></path>
                </svg>
                <span class="text-sm">4 jogadores</span>
            </div>
            <div class="flex items-center space-x-1">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor"
                    stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-calendar h-4 w-4">
                    <path d="M8 2v4"></path>
                    <path d="M16 2v4"></path>
                    <rect width="18" height="18" x="3" y="4" rx="2"></rect>
                    <path d="M3 10h18"></path>
                </svg>
                <span class="text-sm">Há 2 dias</span>
            </div>
        </div>
        <button
            class="inline-flex items-center justify-center gap-2 whitespace-nowrap rounded-md text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 [&amp;_svg]:pointer-events-none [&amp;_svg]:size-4 [&amp;_svg]:shrink-0 h-10 px-4 py-2 w-full bg-rpg-primary hover:bg-rpg-primary/80 text-rpg-text">
            Continuar
        </button>
    </div>
</template>

<style>
</style>