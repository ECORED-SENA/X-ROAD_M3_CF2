<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    .titulo-principal
      .titulo-principal__numero
        span 3
      h1 Guía de implementación

    h2.mb-4 Guía de implementación del ejercicio

    .row.justify-content-center.mb-4
      .col-md-5
        a.anexo.mb-4(:href="obtenerLink('/downloads/anexo1.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p.mb-0 Anexo 1. Guía de Implementación del Ejercicio.

    .row.justify-content-center
      .col-md-6
        figure
          img(src='@/assets/curso/img31.svg', alt='Guía de implementación del ejercicio')

      
  
</template>

<script>
export default {
  name: 'Tema3',
  components: {},
  data: () => ({
    // variables de vue
  }),
}
</script>

<style lang="sass" scoped></style>
