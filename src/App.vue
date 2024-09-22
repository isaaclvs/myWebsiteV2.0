<template>
  <div class="bg-slate-50 min-h-screen font-sans">
    <!-- Header -->
    <header class="bg-cyan-700 p-4 text-white flex flex-col md:flex-row text-center justify-around h-auto">
      <a aria-label="Ir para a página inicial" href="/">
        <img src="./assets/icons/logo.svg" class="w-[2em] mx-5 invert" alt="">
      </a>
      <nav>
        <ul class="flex flex-col md:flex-row justify-center gap-4 mt-1 text-lg font-semibold">
          <li><a href="#sobre" class="hover:text-sky-700">Sobre mim</a></li>
          <li><a href="#projetos" class="hover:text-sky-700">Projetos</a></li>
          <li><a href="#contato" class="hover:text-sky-700">Contato</a></li>
        </ul>
      </nav>
    </header>

    <!-- Seção 'Sobre mim' -->
    <main id="sobre" class="min-h-screen w-auto">
      <div class="bg-cyan-700 flex flex-col md:flex-row justify-around items-center text-center h-auto md:h-[42em]">
        <section class="px-5 md:px-[12em] flex flex-col text-start text-white font-extrabold">
          <p class="text-3xl">Olá!</p>
          <p class="text-5xl md:text-7xl">Eu sou Isaac</p>
          <p class="font-bold">
            Seu resolvedor de problemas.
          </p>
        </section>
        <article>
          <img src="./assets/avatar_original.png" alt="" class="w-32 md:w-auto"/>
        </article>
      </div>
      <div class="flex flex-col md:flex-row justify-between p-10 px-5 md:px-[10rem] divide-x divide-x-2 divide-slate-400 font-semibold">
        <article class="flex flex-col px-5 mb-5 md:mb-0">
          <p>Bem-vindo ao meu mundo! Sou um desenvolvedor full stack apaixonado por criar soluções inovadoras e funcionais. Estou aqui para transformar necessidades em experiências excepcionais.</p>
          <div class="flex gap-4 pt-5 flex-wrap">
            <button
            @click="baixarCurriculo"
            class="bg-cyan-700 hover:bg-cyan-600 text-white font-bold py-3 px-4 md:px-[5rem] gap-2 rounded-lg transition duration-300 ease-in-out shadow-xl flex items-center"
            >
              <img src="./assets/icons/curriculo.svg" alt="Curriculo" class="w-4 h-4 mt-1 invert" />
              Meu currículo
            </button>
            <button
            @click="abrirGithub"
            class="border border-cyan-500 border-2 hover:bg-cyan-700 hover:text-white font-bold py-3 px-4 md:px-[5rem] rounded-lg transition duration-300 ease-in-out shadow-xl flex items-center"
            >
              <img src="./assets/icons/github.svg" alt="Github" class="w-5 h-5 mx-1" />
              Github
            </button>
          </div>
        </article>
        <article class="flex flex-col px-5">
          <p>Meu objetivo é criar experiências digitais que não apenas impressionem, mas também funcionem de forma excepcional e agreguem valor a negócios e projetos ao redor do mundo.</p>
        </article>
      </div>
    </main>

    <!-- Seção 'Projetos' -->
    <section id="projetos" class="p-10">
      <h2 class="text-3xl font-bold text-center">Projetos</h2>
      <div class="mt-6 grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
        <!-- Projeto 1 -->
        <div class="p-6 border rounded-lg bg-gray-50 shadow-xl">
          <h3 class="text-xl font-bold">Projeto 1</h3>
          <p class="mt-2">
            Descrição curta do projeto.
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis nihil atque ab magnam nobis est! Aliquam quia hic commodi nihil molestias error eos dignissimos, tempore laudantium earum voluptates! Expedita, aliquid.
            <a href="#" class="text-blue-500 underline">Veja mais</a>
          </p>
        </div>
        <!-- Projeto 2 -->
        <div class="p-6 border rounded-lg bg-gray-50 shadow-xl">
          <h3 class="text-xl font-bold">Projeto 2</h3>
          <p class="mt-2">
            Descrição curta do projeto.
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Non quasi et optio nisi odio cupiditate recusandae dolor culpa saepe maiores voluptates, explicabo reprehenderit cum aspernatur vero possimus nesciunt adipisci consequuntur?
            <a href="#" class="text-blue-500 underline">Veja mais</a>
          </p>
        </div>
        <!-- Projeto 3 -->
        <div class="p-6 border rounded-lg bg-gray-50 shadow-xl">
          <h3 class="text-xl font-bold">Projeto 3</h3>
          <p class="mt-2">
            Descrição curta do projeto.
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam quae inventore harum enim accusantium modi, ipsam dolore natus sint nam eveniet dolor possimus? Iure dicta est voluptas asperiores, eveniet eos.
            <a href="#" class="text-blue-500 underline">Veja mais</a>
          </p>
        </div>
      </div>
    </section>

    <!-- Seção 'Contato' -->
    <section id="contato" class="py-8">
      <div class="container mx-auto px-5">
        <h2 class="text-3xl font-bold text-center mb-6">Contato</h2>
        
        <div class="p-6 mx-auto gap-5 border rounded-lg bg-gray-50 shadow-xl flex flex-col items-center">
          <!-- LinkedIn -->
          <div class="flex items-center mb-4">
            <img src="./assets/icons/linkedin.svg" alt="LinkedIn" class="w-6 h-6 mr-2" />
            <button @click="abrirLinkedIn" class="text-lg text-gray-800 hover:text-cyan-500">
              LinkedIn
            </button>
          </div>

          <!-- Instagram -->
          <div class="flex items-center mb-4">
            <img src="./assets/icons/instagram.svg" alt="Instagram" class="w-6 h-6 mr-2" />
            <button @click="abrirInstagram" class="text-lg text-gray-800 hover:text-cyan-500">
              Instagram
            </button>
          </div>

          <!-- Email -->
          <div class="flex items-center mb-4">
            <img src="./assets/icons/email.svg" alt="Email" class="w-6 h-6 mr-2" />
            <button @click="abrirEmail" class="text-lg text-gray-800 hover:text-cyan-500">
              dev.isaaclvs@gmail.com
            </button>
          </div>

          <!-- WhatsApp -->
          <div class="flex items-center mb-4">
            <img src="./assets/icons/whatsapp.svg" alt="WhatsApp" class="w-6 h-6 mr-2" />
            <button @click="abrirWhatsApp" class="text-lg text-gray-800 hover:text-cyan-500">
              WhatsApp
            </button>
          </div>

          <!-- Endereço -->
          <div class="flex items-center">
            <img src="./assets/icons/endereco.svg" alt="Endereço" class="w-6 h-6 mr-2" />
            <span class="text-lg text-gray-800">
              Teresina, PI - Brazil
            </span>
          </div>
        </div>
      </div>
    </section>

    <!-- Rodape da pagina -->
    <footer class="bg-gradient-to-b from-cyan-700 bg-cyan-600 text-white py-6 flex flex-col justify-between items-center space-y-6">
      <div class="max-w-3xl px-4 flex items-center justify-between space-x-6 mt-10">
        <p class="font-semibold text-center">
          Fico feliz que tenha chegado até aqui, espero que tenha gostado de saber um pouco sobre mim. 
          Desde que comecei minha trajetória como desenvolvedor, o que mais me atrai é a possibilidade 
          de resolver problemas que parecem sem solução. Se você tem um, fala comigo. Obrigado.
        </p>
        <img src="/images/isaac.jpg" alt="Foto de Isaac Alves" class="w-24 h-24 rounded-full object-cover" />
      </div>
      <div>
        <p class="text-center font-bold">
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
    abrirLinkedIn() {
      window.open('https://www.linkedin.com/in/isaaclvs/', '_blank');
    },
    abrirGithub() {
      window.open('https://www.github.com/isaaclvs/', '_blank');
    },
    abrirEmail() {
      window.open('mailto:dev.isaaclvs@gmail.com', '_self');
    },
    abrirWhatsApp() {
      window.open('https://wa.me/+5586999804586', '_blank');
    },
    abrirInstagram() {
      window.open('https://www.instagram.com/dev.isaaclvs/', '_blank');
    },
    baixarCurriculo() {
      const link = document.createElement('a');
      link.href = './resume/Isaac-Alves.pdf';
      link.download = 'Isaac-Alves.pdf';
      link.click();
    },
  },
};
</script>

<style>

</style>
