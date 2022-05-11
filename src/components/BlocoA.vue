<script>
export default {
  data() {
    return {
      nome: "Bloco A",
      imagem: new URL("./imgs/BlocoA.jpeg", import.meta.url).href,
    };
  },
};
</script>

<template>
  <header>
    <h1>{{ nome }}</h1>
  </header>
  <div>
    <main id="content">
      <div class="lacunas">
        <p>Gabinete</p>
        <p>Direção Geral</p>
        <p>Auditoria Cooperação de Cooperativismo</p>
        <p>Dape Departamento de Administração e Planejamento</p>
        <p>Sanitário masculino</p>
        <p>Sanitário Feminino</p>
        <p>Laboratório do Olhar</p>
        <p>A-01 Sala de Aula</p>
        <p>A-02 Sala de Aula</p>
        <p>A-03 Sala de Aula</p>
        <p>A-04 Sala de Aula</p>
        <p>A-05 Sala de Aula</p>
        <p>A-06 Sala de Professores Fernando, Sérgio</p>
        <p>A-07 Laboratório de Agrimensura</p>
        <p>A-08 Laboratório Química</p>
        <p>A-09 Laboratório de Biologia</p>
        <p>A-10 Arquivo RaCi</p>
        <p>A-11 Laboratório de Informática</p>
        <p>A-12 Laboratório de Hardware e Arquitetura de Computadores</p>
        <p>A-13 Coordenação de Gestão de Pessoas</p>
      </div>
      <div>
        <img :src="imagem" alt="" />
      </div>
      <div class="lacunas">
        <p>A-14 Sala de Professores Garciela, Jaqueline, Luana, Neiva, Lúcia</p>
        <p>
          A-15 Sala de Professores Greice, Alessandra, Marcelo, Patrícia e
          Renilse
        </p>
        <p>A-16 Sala de Professores Clodoaldo, Luiz, Leandro, Jean</p>
        <p>A-18/17 Registro Acadêmico/Secretaria</p>
        <p>A-19 Sala de Reunião Direção Geral</p>
        <p>A-19d Sala de Direção</p>
        <p>A-20 Copa</p>
        <p>A-21 Sala de Professores Alceu, Casemiro, Fernanda, Luiz, Paulo</p>
        <p>A-22 Arquivo Morto</p>
        <p>
          A-23 Coordenação de Pós-Graduação, Sala de Reuniçao, DDE, CGG,
          Coordenação de Agronomia, Eja, CECOM, Pesquisa e Extensão
        </p>
        <p>A-24</p>
        <p>
          A-25 Sala de Professores Ana Cristina, Luci, Marilene, Ricicler,
          Sueli, Griscele, Sandro
        </p>
        <p>A-26 Licitações e Contrato</p>
        <p>A-27</p>
        <p>A-28 Depósito</p>
      </div>
    </main>
  </div>

  <input id="menu-projeto" type="checkbox" />
  <label for="menu-projeto">
    <div class="menu">
      <span class="projeto"></span>
    </div>
  </label>

  <ul>
    <li @click="$emit('altera-atual', 'campus')">Início</li>
    <li @click="$emit('altera-atual', 'campus')">Bloco A</li>
    <li @click="$emit('altera-atual', 'campus')">Bloco B</li>
    <li @click="$emit('altera-atual', 'campus')">Bloco C</li>
    <li @click="$emit('altera-atual', 'campus')">Bloco D</li>
    <li @click="$emit('altera-atual', 'campus')">Bloco E</li>
    <li @click="$emit('altera-atual', 'campus')">Ginásio</li>
    <li @click="$emit('altera-atual', 'campus')">Encubatório</li>
    <li @click="$emit('altera-atual', 'campus')">Fazenda</li>
  </ul>
</template>
