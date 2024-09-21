<template>
  <div class="bg-slate-50 min-h-screen font-sans">
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
          <div class="flex gap-4 pt-5">
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
    <section id="projetos" class="p-10 mt-10">
      <h2 class="text-3xl font-bold text-center">Projetos</h2>
      <div class="mt-6 grid grid-cols-1 md:grid-cols-3 gap-6">
        <!-- Projeto 1 -->
        <div class="p-6 border rounded-lg bg-gray-50 shadow-xl">
          <h3 class="text-xl font-bold">Projeto 1</h3>
          <p class="mt-2">
            Descrição curta do projeto.{' Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sed vero, minus impedit repellendus id a sint voluptatum voluptate autem ducimus culpa. Laboriosam amet excepturi voluptas consequatur perferendis quaerat repellendus facilis?Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quibusdam suscipit totam magni consectetur labore in voluptatem voluptate voluptas neque corporis veritatis molestias recusandae, accusamus, deserunt laborum. Repellat excepturi esse dignissimos? '}
            <a href="#" class="text-blue-500 underline">Veja mais</a>
          </p>
        </div>
        <!-- Projeto 2 -->
        <div class="p-10 border rounded-lg bg-gray-50 shadow-xl">
          <h3 class="text-xl font-bold">Projeto 2</h3>
          <p class="mt-2">
            Descrição curta do projeto.{' Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sed vero, minus impedit repellendus id a sint voluptatum voluptate autem ducimus culpa. Laboriosam amet excepturi voluptas consequatur perferendis quaerat repellendus facilis?Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quibusdam suscipit totam magni consectetur labore in voluptatem voluptate voluptas neque corporis veritatis molestias recusandae, accusamus, deserunt laborum. Repellat excepturi esse dignissimos? '}
            <a href="#" class="text-blue-500 underline">Veja mais</a>
          </p>
        </div>
        <!-- Projeto 3 -->
        <div class="p-6 border rounded-lg bg-gray-50 shadow-xl">
          <h3 class="text-xl font-bold">Projeto 3</h3>
          <p class="mt-2">
            Descrição curta do projeto.{' Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sed vero, minus impedit repellendus id a sint voluptatum voluptate autem ducimus culpa. Laboriosam amet excepturi voluptas consequatur perferendis quaerat repellendus facilis?Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quibusdam suscipit totam magni consectetur labore in voluptatem voluptate voluptas neque corporis veritatis molestias recusandae, accusamus, deserunt laborum. Repellat excepturi esse dignissimos? '}
            <a href="#" class="text-blue-500 underline">Veja mais</a>
          </p>
        </div>
        <!-- Futuros projetos aqui -->
      </div>
    </section>

    <!-- Seção 'Contato' -->
    <section class="py-8">
      <div class="container mx-auto px-10">
        <h2 class="text-3xl font-bold text-center mb-6">Contato</h2>
        
        <div class="p-6 mx-10 gap-5 border rounded-lg bg-gray-50 shadow-xl flex flex-col items-center">
          <!-- Email -->
          <div class="flex items-center mb-4">
            <img src="caminho/para/icone-email.svg" alt="Email" class="w-6 h-6 mr-2" />
            <button @click="abrirEmail" class="text-lg text-gray-800 hover:text-blue-500">
              Email
            </button>
          </div>

          <!-- WhatsApp -->
          <div class="flex items-center mb-4">
            <img src="caminho/para/icone-whatsapp.svg" alt="WhatsApp" class="w-6 h-6 mr-2" />
            <button @click="abrirWhatsApp" class="text-lg text-gray-800 hover:text-blue-500">
              WhatsApp
            </button>
          </div>

          <!-- LinkedIn -->
          <div class="flex items-center mb-4">
            <img src="caminho/para/icone-linkedin.svg" alt="LinkedIn" class="w-6 h-6 mr-2" />
            <button @click="abrirLinkedIn" class="text-lg text-gray-800 hover:text-blue-500">
              LinkedIn
            </button>
          </div>

          <!-- Instagram -->
          <div class="flex items-center mb-4">
            <img src="caminho/para/icone-instagram.svg" alt="Instagram" class="w-6 h-6 mr-2" />
            <button @click="abrirInstagram" class="text-lg text-gray-800 hover:text-blue-500">
              Instagram
            </button>
          </div>

          <!-- Endereço -->
          <div class="flex items-center">
            <img src="caminho/para/icone-endereco.svg" alt="Endereço" class="w-6 h-6 mr-2" />
            <span class="text-lg text-gray-800">
              Teresina, PI - Brazil
            </span>
          </div>
        </div>
      </div>
    </section>

    <!-- Rodape da pagina -->
    <footer class="bg-blue-500 text-white py-4">
      <div class="container mx-auto px-4">
        <!-- Texto de Lorem Ipsum -->
        <p class="text-center mb-4">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque at lorem vitae purus vehicula sollicitudin.
        </p>
        <!-- Texto de Copyright -->
        <p class="text-center font-semibold">
          &copy; 2024 Isaac Alves. Todos os direitos reservados.
        </p>
      </div>
    </footer>
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
    abrirEmail() {
      window.open('mailto:dev.isaaclvs@gmail.com', '_self');
    },
    abrirWhatsApp() {
      window.open('https://wa.me/+5586999804586', '_blank');
    },
    abrirLinkedIn() {
      window.open('https://www.linkedin.com/in/isaaclvs', '_blank');
    },
    abrirInstagram() {
      window.open('https://www.instagram.com/dev.isaaclvs/', '_blank');
    },
  },
};
</script>

<style>

</style>
