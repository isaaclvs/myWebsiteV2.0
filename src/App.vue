<template>
  <div class="bg-gray-100 min-h-screen font-sans">
    <!-- Header -->
    <header class="bg-blue-600 p-6 text-white text-center">
      <h1 class="text-4xl font-bold">Isaac Alves</h1>
      <p class="mt-2 text-lg">Engenheiro de Software | Ruby e Java</p>
      <nav class="mt-4">
        <a href="#sobre" class="mx-4 hover:underline">Sobre mim</a>
        <a href="#projetos" class="mx-4 hover:underline">Projetos</a>
        <a href="#contato" class="mx-4 hover:underline">Contato</a>
      </nav>
    </header>

    <!-- Seção 'Sobre mim' -->
    <section id="sobre" class="p-10 text-center">
      <h2 class="text-3xl font-bold">Sobre mim</h2>
      <p class="mt-4 text-gray-700">
        Desenvolvedor web especializado em Ruby e Java, com experiência em
        criação de aplicações modernas e escaláveis.
      </p>
    </section>

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
};
</script>

<style>
/* ... */
</style>
