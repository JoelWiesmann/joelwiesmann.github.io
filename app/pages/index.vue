<template>
    <div>
        <UCard class="m-10 shadow-2xl">
            <div class="sm:flex justify-between">
                <div>
                    <h1 class="text-2xl font-bold">wiesmann.io</h1>
                </div>
                <div>
                    <UIcon :name="icon" @click="colorModeToggle"></UIcon>
                </div>
            </div>
            <div class="sm:flex">
                <div class="text-center">
                    <NuxtImg src="images/joel.png" class="w-80" />
                    <i>Me, thinking about life and stuff.</i>
                </div>
                <div class="sm:w-1/2 text-justify">
                    <br />
                    Welcome to my domain!<br />
                    <br />
                    I'm an experienced automation engineer from Switzerland 🫕 with a passion for Broadcom Automic,
                    Python, Bash and GenAI technologies.<br />
                    <br />
                    Also I'm a content creator / trainer at Philipp Elmer Membership (<NuxtLink
                        href="https://www.pemautomic.com" target="_blank">en</NuxtLink> / <NuxtLink
                        href="https://membership.philippelmer.com" target="_blank">de</NuxtLink>).<br />
                    <br />
                    However, I don't want to spread my personal details all over the internet. If you want to get in
                    touch with me, you can connect with me on LinkedIn.<br />
                    <br />
                    - Joel<br />
                    <br />
                    <NuxtLink href="https://www.linkedin.com/in/joel-wiesmann/" target="_blank">
                        <i class="fab fa-linkedin fa-2x"></i>
                    </NuxtLink>
                </div>
            </div>
        </UCard>
    </div>
</template>

<script setup>
const colormode = useColorMode()

const icon = computed(() => colormode.value === 'dark' ? 'i-heroicons-sun' : 'i-heroicons-moon')
const colorModeToggle = () => colormode.value = colormode.value === 'dark' ? 'light' : 'dark'

</script>