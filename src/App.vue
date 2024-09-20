<template>
  <div class="bg-gray-100 min-h-screen font-sans">
    <!-- Header -->
    <header class="bg-blue-500 p-4 text-white flex text-center justify-around">
      <a aria-label="Ir para a página inicial" href="/">
        <img src="./assets/logo.png" class="w-[2em] mx-5 invert" alt="">
      </a>
      <nav>
        <ul class="flex justify-between gap-4 mx-7 mt-1 text-lg font-semibold">
          <li><a href="#sobre" class="hover:bg-sky-700">Sobre mim</a></li>
          <li><a href="#projetos" class="hover:bg-sky-700">Projetos</a></li>
          <li><a href="#contato" class="hover:bg-sky-700">Contato</a></li>
        </ul>
      </nav>
    </header>

    <!-- Seção 'Sobre mim' -->
    <main id="sobre" class="">
      <div class="bg-blue-500 flex justify-around text-center">
        <section class="h-[500px] w-[500px] pl-[50px] flex flex-col text-start text-white pt-[250px] font-extrabold">
          <p class="text-3xl">Olá!</p>
          <p class="text-7xl">Eu sou Isaac</p>
          <p class="font-bold">
            Muito prazer, resolvedor de problemas.
          </p>
        </section>
        <article>
          <img src="./assets/avatar_original.png" alt="">
        </article>
      </div>
      <div class="h-[10rem] flex justify-between p-7 px-[10rem] pt-[70px] divide-x divide-x-2 divide-slate-400 font-semibold">
        <article class="flex flex-row flex-col px-5">
          <p>Bem-vindo ao meu mundo! Sou um desenvolvedor full stack apaixonado por criar soluções inovadoras e funcionais. Estou aqui para transformar necessidades em experiências excepcionais.</p>
          <br>
          <div class="flex gap-4">
            <button
            @click="irParaLinkedIn"
            class="bg-blue-500 hover:bg-blue-600 text-white font-bold py-3 px-[5rem] gap-2 rounded-lg transition duration-300 ease-in-out shadow-xl flex"
            >
              <img src="./assets/linkedin.png" alt="LinkedIn" class="w-4 h-4 mt-1 invert" />
              LinkedIn
            </button>
            <button
            @click="irParaGithub"
            class="border border-blue-500 border-2 hover:bg-blue-500 hover:text-white font-bold py-3 px-[5rem] rounded-lg transition duration-300 ease-in-out shadow-xl flex"
            >
              <img src="./assets/github.png" alt="Github" class="w-5 h-5 mx-1" />
              Github
            </button>
          </div>
        </article>
        <article class="flex flex-row px-5">
          <p>Meu objetivo é criar experiências digitais que não apenas impressionem, mas também funcionem de forma excepcional e agreguem valor a negócios e projetos ao redor do mundo.</p>
        </article>
      </div>
    </main>

    <!-- Seção 'Projetos' -->
    <section id="projetos" class="p-10 bg-white">
      <h2 class="text-3xl font-bold text-center">Projetos</h2>
      <div class="mt-6 grid grid-cols-1 md:grid-cols-3 gap-6">
        <div class="p-6 border rounded-lg bg-gray-50">
          <h3 class="text-xl font-bold">Projeto 1</h3>
          <p class="mt-2">
            Descrição curta do projeto.{' '}
            <a href="#" class="text-blue-500 underline">Veja mais</a>
          </p>
        </div>
        <!-- Adicione mais projetos aqui -->
      </div>
    </section>

    <!-- Seção 'Contato' -->
    <section id="contato" class="p-10 text-center bg-gray-100">
      <h2 class="text-3xl font-bold">Contato</h2>
      <p class="mt-4 text-gray-700">
        Entre em contato comigo através das redes sociais ou envie uma mensagem.
      </p>
      <div class="mt-6">
        <a href="https://www.linkedin.com/in/isaac-alves" class="text-blue-600 underline mx-2">
          LinkedIn
        </a>
        <a href="https://github.com/isaac-alves" class="text-blue-600 underline mx-2">
          GitHub
        </a>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'App',
  methods: {
    irParaLinkedIn() {
      window.open('https://www.linkedin.com/in/isaaclvs/', '_blank');
    },
    irParaGithub() {
      window.open('https://www.github.com/isaaclvs/', '_blank');
    },
  },
};
</script>

<style>
/* ... */
</style>
