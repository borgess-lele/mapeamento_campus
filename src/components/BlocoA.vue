<template>
  <header><h1>Bloco A</h1></header>
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
