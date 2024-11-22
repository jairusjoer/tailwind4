<script setup lang="ts">
import ThemeTest from './components/ThemeTest.vue'
</script>

<template>
    <header class="p-4">
        <h1 class="font-bold">Tailwind CSS 4</h1>
    </header>
    <main>
        <ThemeTest />
        <ThemeTest title="Dark Mode" class="dark-mode bg-background text-foreground-subtle">
            <ThemeTest title="Light Mode" class="light-mode bg-background text-foreground-subtle">
                <ThemeTest title="Dark Mode" class="dark-mode bg-background text-foreground-subtle" />
            </ThemeTest>
        </ThemeTest>
    </main>
</template>
