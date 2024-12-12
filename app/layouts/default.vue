<template>
    <div class="container mx-auto max-w-4xl">
        <main class="my-10">
            <slot />
        </main>
    </div>
</template>

<script setup>
useHead({
    title: 'wiesmann.io',
    icon: 'images/favicon.svg',
    bodyAttrs: {
        class: 'bg-gray-800',
    },
    meta: [
        {
            name: 'description',
            content: 'Joel Wiesmann - AI / Automation Engineer & Automic expert from Switzerland',
        },
    ],
    link: [
        {
            rel: 'preconnect',
            href: 'https://fonts.googleapis.com',
        },
        {
            rel: 'stylesheet',
            href: 'https://fonts.googleapis.com/css2?family=Inter&display=swap',
        },
    ],
})
</script>
