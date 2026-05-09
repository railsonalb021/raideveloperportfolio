<script setup lang="ts">
</script>

<template>
  <section
    id="principal"
    class="min-h-screen text-white px-6 flex flex-col items-center justify-center overflow-x-hidden"
  >
    <div class="absolute w-[400px] h-[500px] bg-orange-800/20 blur-[120px] rounded-full top-20 left-1/2 -translate-x-1/2" />

    <div class="relative flex flex-col items-center text-center max-w-3xl">

      <h1 class="text-5xl md:text-6xl font-bold mb-4 leading-tight">
        rai<span class="text-orange-600">.developer</span>
      </h1>

      <p class="text-lg md:text-xl text-gray-400 mb-8">
        Criando interfaces modernas, rápidas e interativas com Vue, Tailwind e TypeScript.
      </p>

      <div class="flex gap-4 flex-wrap justify-center">
        
          <button
            class="bg-orange-700 hover:bg-orange-600 px-6 py-2 rounded-full font-semibold transition-all duration-300 hover:scale-105"
          >
            Ver Projetos
          </button>

        <button
          class="border border-zinc-700 hover:border-orange-500 px-6 py-3 rounded-full font-semibold text-gray-300 hover:text-white transition-all duration-300"
        >
          Sobre mim
        </button>
      </div>

      <div class="mt-16 grid grid-cols-3 gap-8 text-center">
        <div>
          <h2 class="text-2xl font-bold text-orange-700">+3</h2>
          <p class="text-gray-400 text-sm">Projetos</p>
        </div>

        <div>
          <h2 class="text-2xl font-bold text-orange-700">+3</h2>
          <p class="text-gray-400 text-sm">Anos estudando</p>
        </div>

        <div>
          <h2 class="text-2xl font-bold text-orange-700">100%</h2>
          <p class="text-gray-400 text-sm">Foco em Front-end</p>
        </div>
      </div>
    </div>
  </section>
  
  <section
  id="projetos"
  class="min-h-screen text-white px-6 flex flex-col items-center"
>
  <h1 class="text-5xl md:text-4xl font-extralight mb-14 leading-tight">
    Meus<span class="text-orange-700"> Projetos</span>
  </h1>

  <div class="grid grid-cols-1 md:grid-cols-2 xl:grid-cols-3 gap-8 max-w-7xl w-full">

    <div
      class="group relative overflow-hidden rounded-3xl border border-zinc-800 bg-zinc-900/60 backdrop-blur-sm p-6 transition-all duration-500 hover:-translate-y-2 hover:border-orange-700 hover:shadow-[0_0_40px_rgba(234,88,12,0.15)]"
    >
      <div
        class="absolute inset-0 bg-gradient-to-br from-orange-700/10 to-transparent opacity-0 group-hover:opacity-100 transition duration-500"
      />

      <div class="relative z-10">
        <div
          class="w-14 h-14 rounded-2xl bg-orange-700/20 border border-orange-700/30 flex items-center justify-center mb-6"
        >
          <Icon name="mdi:hammer" class="text-3xl text-orange-500" />
        </div>

        <h2 class="text-2xl font-bold mb-3">
          Marcenaria Maranhão
        </h2>

        <p class="text-gray-400 leading-relaxed mb-6">
          Site de marcenaria desenvolvido com foco em apresentação profissional,
          design moderno e experiência responsiva.
        </p>

        <div class="flex gap-3">
          <NuxtLink
            to="https://marcenaria-maranhao.vercel.app/"
            class="rounded-xl font-medium transition-all duration-300 hover:scale-105" target="_blank">
            <Icon name="mdi:link" class="text-3xl text-white hover:text-orange-500 transition-all ease-out duration-300" />
          </NuxtLink>
 
          <NuxtLink
            to="https://github.com/railsonalb021/marcenaria-maranhao"
            class="rounded-xl font-medium transition-all duration-300 hover:scale-105" target="_blank">
          <Icon name="mdi:github" class="text-3xl text-white hover:text-orange-500 transition-all ease-out duration-300" />
          </NuxtLink>
        </div>
      </div>
    </div>

    <div
      class="group relative overflow-hidden rounded-3xl border border-zinc-800 bg-zinc-900/60 backdrop-blur-sm p-6 transition-all duration-500 hover:-translate-y-2 hover:border-orange-700 hover:shadow-[0_0_40px_rgba(234,88,12,0.15)]"
    >
      <div
        class="absolute inset-0 bg-gradient-to-br from-orange-700/10 to-transparent opacity-0 group-hover:opacity-100 transition duration-500"
      />

      <div class="relative z-10">
        <div
          class="w-14 h-14 rounded-2xl bg-orange-700/20 border border-orange-700/30 flex items-center justify-center mb-6"
        >
          <Icon name="mdi:school" class="text-3xl text-orange-500" />
        </div>

        <h2 class="text-2xl font-bold mb-3">
          Teacher Nay
        </h2>

        <p class="text-gray-400 leading-relaxed mb-6">
          Site desenvolvido para divulgação das aulas de inglês,
          com visual moderno e foco na apresentação profissional.
        </p>

        <div class="flex gap-3">

          <NuxtLink
            to="https://teachernay.vercel.app/"
            class="rounded-xl font-medium transition-all duration-300 hover:scale-105" target="_blank">
            <Icon name="mdi:link" class="text-3xl text-white hover:text-orange-500 transition-all ease-out duration-300" />
          </NuxtLink>

          <NuxtLink
            to="https://github.com/railsonalb021/teachernay"
            class="rounded-xl font-medium transition-all duration-300 hover:scale-105" target="_blank">
          <Icon name="mdi:github" class="text-3xl text-white hover:text-orange-500 transition-all ease-out duration-300" />
          </NuxtLink>
        </div>
      </div>
    </div>

    <div
      class="group relative overflow-hidden rounded-3xl border border-zinc-800 bg-zinc-900/60 backdrop-blur-sm p-6 transition-all duration-500 hover:-translate-y-2 hover:border-orange-700 hover:shadow-[0_0_40px_rgba(234,88,12,0.15)] mb-20 md:mb-0"
    >
      <div
        class="absolute inset-0 bg-gradient-to-br from-orange-700/10 to-transparent opacity-0 group-hover:opacity-100 transition duration-500"
      />

      <div class="relative z-10">
        <div
          class="w-14 h-14 rounded-2xl bg-orange-700/20 border border-orange-700/30 flex items-center justify-center mb-6"
        >
          <Icon name="mdi:code-tags" class="text-3xl text-orange-500" />
        </div>

        <h2 class="text-2xl font-bold mb-3">
          Meu Portfólio
        </h2>

        <p class="text-gray-400 leading-relaxed mb-6">
          Meu portfólio pessoal desenvolvido para apresentar projetos,
          habilidades e experiências de forma moderna e responsiva.
        </p>

        <div class="flex gap-3">
          <NuxtLink
            to="https://raideveloperportfolio.vercel.app/"
            class="rounded-xl font-medium transition-all duration-300 hover:scale-105" target="_blank">
            <Icon name="mdi:link" class="text-3xl text-white hover:text-orange-500 transition-all ease-out duration-300" />
          </NuxtLink>
 
          <NuxtLink
            to="https://github.com/railsonalb021/raideveloperportfolio"
            class="rounded-xl font-medium transition-all duration-300 hover:scale-105" target="_blank">
          <Icon name="mdi:github" class="text-3xl text-white hover:text-orange-500 transition-all ease-out duration-300" />
          </NuxtLink>
        </div>
      </div>
    </div>
  </div>
</section>
</template>