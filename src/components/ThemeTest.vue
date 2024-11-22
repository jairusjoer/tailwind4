<script setup lang="ts">
const { title = 'Default' } = defineProps<{
    title: string
}>();
</script>

<template>
    <section class="p-4 space-y-4">
        <h2 class="font-bold">{{ title }}</h2>
        <div class="flex flex-wrap gap-4">
            <!-- Neutral -->
            <button class="bg-neutral text-neutral-subtle">Neutral</button>
            <button class="bg-neutral-subtle text-neutral">Neutral</button>
            <!-- Brand -->
            <button class="bg-brand text-brand-subtle">Brand</button>
            <button class="bg-brand-subtle text-brand">Brand</button>
            <!-- Informative -->
            <button class="bg-informative text-informative-subtle">Informative</button>
            <button class="bg-informative-subtle text-informative">Informative</button>
            <!-- Successful -->
            <button class="bg-successful text-successful-subtle">Successful</button>
            <button class="bg-successful-subtle text-successful">Successful</button>
            <!-- Cautionary -->
            <button class="bg-cautionary text-cautionary-subtle">Cautionary</button>
            <button class="bg-cautionary-subtle text-cautionary">Cautionary</button>
            <!-- Destructive -->
            <button class="bg-destructive text-destructive-subtle">Destructive</button>
            <button class="bg-destructive-subtle text-destructive">Destructive</button>
            <!-- Inputs -->
            <input type="text">
        </div>
        <slot />
    </section>
</template>