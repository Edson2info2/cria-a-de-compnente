<script>
export default {
  props: {
    titulo: {
      default: "Titulo Padrão",
    },
    nomes: {
      type: Array,
    },
  },
};
</script>

<template>
  <article class="block">
    {{ titulo }}
    <hr />
    <ul>
      <li v-for="(nome, i) of nomes" :key="i"></li>
      {{
        nome
      }}
    </ul>
  </article>
</template>
