<script>
import BlocoCampus from "@/components/BlocoCampus.vue";
import BlocoA from "@/components/BlocoA.vue";
import BlocoB from "@/components/BlocoB.vue";
import BlocoC from "@/components/BlocoC.vue";
import BlocoD from "@/components/BlocoD.vue";
import BlocoE from "@/components/BlocoE.vue";
import BlocoEncubatorio from "@/components/BlocoEncubatorio.vue";
import BlocoGinasio from "@/components/BlocoGinasio.vue";
import BlocoFazenda from "@/components/BlocoFazenda.vue";

export default {
  components: {
    BlocoCampus,
    BlocoA,
    BlocoB,
    BlocoC,
    BlocoD,
    BlocoE,
    BlocoEncubatorio,
    BlocoGinasio,
    BlocoFazenda,
  },
  data() {
    return {
      atual: "BlocoA",
    };
  },
  methods: {
    alteraAtual(valor) {
      this.atual = valor;
    },
  },
};
</script>

<template>
  <BlocoCampus
    v-if="atual === 'campus'"
    @altera-atual="alteraAtual"
  ></BlocoCampus>
  <BlocoA v-if="atual === 'BlocoA'" @altera-atual="alteraAtual"></BlocoA>
  <BlocoB v-if="atual === 'BlocoB'" @altera-atual="alteraAtual"></BlocoB>
  <BlocoC v-if="atual === 'BlocoC'" @altera-atual="alteraAtual"></BlocoC>
  <BlocoD v-if="atual === 'BlocoD'" @altera-atual="alteraAtual"></BlocoD>
  <BlocoE v-if="atual === 'BlocoE'" @altera-atual="alteraAtual"></BlocoE>
  <BlocoEncubatorio
    v-if="atual === 'BlocoEncubatorio'"
    @altera-atual="alteraAtual"
  ></BlocoEncubatorio>
  <BlocoGinasio
    v-if="atual === 'BlocoGinasio'"
    @altera-atual="alteraAtual"
  ></BlocoGinasio>
  <BlocoFazenda
    v-if="atual === 'BlocoFazenda'"
    @altera-atual="alteraAtual"
  ></BlocoFazenda>
</template>

<style></style>
