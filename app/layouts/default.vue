<script setup lang="ts"></script>

<template>
    <Navbar />
    <main class="min-h-screen bg-gradient-to-b from-zinc-950 via-zinc-900 to-zinc-950 overflow-x-hidden">
        <slot />
    </main>
    <Footer />
</template>