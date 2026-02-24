<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    p.mb-5 La siguiente imagen presenta una síntesis de las temáticas estudiadas en el componente formativo.
    .row.justify-content-center
      .col-lg-10.mb-5
        figure
          img(src="@/assets/curso/temas/sintesis-2.svg", alt="A continuación, se presenta la síntesis del componente formativo: Estructura de documentos en la cual se encuentra: Gestión documental. Desarrollo administrativo. Categorías gramaticales como lo son los sustantivos, adjetivos, verbos, adverbios, determinantes, pronombres, preposiciones, conjunciones e interjecciones. Clases de oraciones, entre ellas, según la intención del hablante, la estructura del predicado y la cantidad de verbos. Párrafo, siendo estos, descriptivos, narrativos y argumentativos. Signos de puntuación, teniendo: punto, coma, punto y coma, dos puntos, comillas, paréntesis, signos de interrogación, signos de exclamación, puntos suspensivos y raya.")
      .col-auto
        a.anexo.mb-4(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis

</template>

<script>
export default {
  name: 'Sintesis',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
