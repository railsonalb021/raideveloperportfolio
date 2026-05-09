<script setup lang="ts">
import { ref } from 'vue'

const isOpen = ref(false)

const toggleMenu = () => {
  isOpen.value = !isOpen.value
}
</script>

<template>
  <div class="flex justify-end items-center">
    <button
    class="md:hidden fixed top-4 right-12 z-[60] text-white bg-zinc-900 px-2 py-2 rounded-md border border-zinc-700"
    @click="toggleMenu"
  >
    <Icon :name="isOpen ? 'mdi:close' : 'mdi:menu'" class="text-2xl flex" />
  </button>
  </div>

  <div
    v-if="isOpen"
    class="fixed inset-0 bg-black/60 z-40 md:hidden transition-opacity duration-300"
    @click="toggleMenu"
  />

  <aside
    class="hidden md:flex fixed left-0 top-0 h-screen w-20 bg-zinc-900 border-r border-zinc-800 flex-col items-center py-6 z-50"
  >
    <div class="mb-10">
      <img
        src="/fotoperfil.png"
        alt="Foto de perfil"
        class="w-12 h-12 rounded-full object-cover hover:scale-110 transition duration-300"
      />
    </div>

    <div class="flex flex-col gap-10 mt-10">
      <NuxtLink to="#principal" class="text-gray-400 hover:text-orange-600 transition-all duration-300">
        <Icon name="mdi:home" class="icon" />
      </NuxtLink>

      <NuxtLink to="https://github.com/railsonalb021" target="_blank" class="text-gray-400 hover:text-orange-600 transition-all duration-300">
        <Icon name="mdi:github" class="icon" />
      </NuxtLink>

      <NuxtLink to="https://www.linkedin.com/in/railson-albino-40785b259/" target="_blank" class="text-gray-400 hover:text-orange-600 transition-all duration-300">
        <Icon name="mdi:linkedin" class="icon" />
      </NuxtLink>

      <Icon name="mdi:youtube" class="icon" />

      <NuxtLink to="https://www.instagram.com/rai.albb/" target="_blank" class="text-gray-400 hover:text-orange-600 transition-all duration-300">
        <Icon name="mdi:instagram" class="icon" />
      </NuxtLink>

      <Icon name="mdi:twitter" class="icon" />

      <NuxtLink to="mailto:railsonaov@gmail.com" target="_blank" class="text-gray-400 hover:text-orange-600 transition-all duration-300">
        <Icon name="mdi:email" class="icon" />
      </NuxtLink>
    </div>
  </aside>

  <aside
    class="fixed top-0 left-0 h-screen w-20 bg-zinc-900 border-r border-zinc-800 z-50 md:hidden
    transform transition-transform duration-300 ease-in-out"
    :class="isOpen ? 'translate-x-0' : '-translate-x-full'"
  >
    <div class="flex flex-col items-center py-6">
      <img
        src="/fotoperfil.png"
        alt="Foto de perfil"
        class="w-14 h-14 rounded-full object-cover mb-10"
      />

      <div class="flex flex-col gap-8 text-center">
        <NuxtLink @click="toggleMenu" to="#principal" class="text-gray-400 hover:text-orange-600">
          <Icon name="mdi:home" class="icon" />
        </NuxtLink>

        <NuxtLink @click="toggleMenu" to="https://github.com/railsonalb021" target="_blank" class="text-gray-400 hover:text-orange-600">
          <Icon name="mdi:github" class="icon" />
        </NuxtLink>

        <NuxtLink @click="toggleMenu" to="https://www.linkedin.com/in/railson-albino-40785b259/" target="_blank" class="text-gray-400 hover:text-orange-600">
          <Icon name="mdi:linkedin" class="icon" />
        </NuxtLink>

        <Icon name="mdi:youtube" class="icon" />

        <NuxtLink @click="toggleMenu" to="https://www.instagram.com/rai.albb/" target="_blank" class="text-gray-400 hover:text-orange-600">
          <Icon name="mdi:instagram" class="icon" />
        </NuxtLink>

        <Icon name="mdi:twitter" class="icon" />

        <NuxtLink @click="toggleMenu" to="mailto:railsonaov@gmail.com" target="_blank" class="text-gray-400 hover:text-orange-600">
          <Icon name="mdi:email" class="icon" />
        </NuxtLink>
      </div>
    </div>
  </aside>
</template>

<style scoped>
.icon {
  @apply text-3xl text-gray-400 hover:text-orange-600 transition-all duration-300 cursor-pointer hover:scale-110;
}
</style>