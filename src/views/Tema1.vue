<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    .titulo-principal
      .titulo-principal__numero
        span 1
      h1 Escalabilidad y alta disponibilidad
    
    figure.mb-5
      img(src='@/assets/curso/img11.png', alt='Escalabilidad y alta disponibilidad')
    
    #t1_1.titulo-segundo
      h2 1.1 Rendimiento

    .row.mb-5.align-items-center
      .col-lg-8    
        p.mb-4
          | Capacidad de un sistema de software de responder ante los 
          strong requisitos de tiempo, 
          | teniendo en cuenta que:
        
        ol.lista-ol--cuadro
          li 
            .lista-ol--cuadro__vineta
              span 1
            | Las tareas que realizan los sistemas se han vuelto mucho más complejas con el tiempo.
          li 
            .lista-ol--cuadro__vineta
              span 2
            | Las solicitadas realizadas a un sistema (en términos de complejidad, número de transacciones, número de usuarios, entre otros) también han crecido de formas que hubieran sido inimaginables en años anteriores.
      .col-lg-4
        figure
          img(src='@/assets/curso/img12.svg', alt='Escalabilidad y alta disponibilidad')
    
    #t1_2.titulo-segundo
      h2 1.2 Escalabilidad

    p.mb-4 
      | Capacidad de un sistema de software para 
      strong permanecer en funcionamiento 
      | en los escenarios en los que hay un incremento de usuarios, transacciones y/o datos.

    .row.mb-4.justify-content-center
      .col-md-8.col-lg-4
        h4.ConTitle Objetivo
    
    .row.justify-content-center.mb-5
      .col-lg-5
        .tarjeta-avatar-b.mb-5
          img(src='@/assets/curso/img14.svg' alt='Aumentar')
          .tarjeta.tarjeta--azul
            .p-4
              .h3 Aumentar el «Throughput»
              p 
                | Cantidad de 
                strong carga de trabajo 
                | que un sistema de software es capaz de manejar en un período de tiempo unitario.
              p.mb-0 
                strong Unidad: 
                | transacciones / minuto.
      
      .col-lg-5
        .tarjeta-avatar-b.mb-5
          img(src='@/assets/curso/img13.svg' alt='Disminuir')
          .tarjeta.tarjeta--azul
            .p-4
              .h3 Disminuir el tiempo de respuesta
              p 
                strong Tiempo que tarda 
                | en completarse una interacción específica con un sistema de software.
              p.mb-0
                strong Unidad: 
                | milisegundos (ms).

    #t1_3.titulo-segundo
      h2 1.3 Alta disponibilidad
    
    p.mb-5
      | Capacidad de un sistema de software para estar completamente operativo 
      strong cuando sea necesario.
    
    .row.mb-5.justify-content-center
      .col-lg-5
        .row.mb-4
          .col-lg-10
            h4.ConTitle Objetivo
        p.mb-1 
          | Eliminar cualquier tipo de SPOF 
          strong (Single Point of Failure): 
        p Punto único de falla.
      .col-lg-5
        figure
          img(src='@/assets/curso/img15.svg', alt='Alta disponibilidad')
    
    #t1_4.titulo-segundo
      h2 1.4 Táctica arquitectónica de escalamiento
    
    .row.gx-5.mb-5
      .col-md-6
        .p-5.Bg01
          h3 Escalamiento vertical
          p.mb-4 Aumenta la capacidad del sistema de software existente, aumentando las características de hardware en el mismo servidor.
          h4.mb-4 Consideraciones:
          ol.lista-ol--cuadro.mb-4
            li 
              .lista-ol--cuadro__vineta
                span 1
              | Inversión adicional.
            li 
              .lista-ol--cuadro__vineta
                span 2
              | Existencia de un único punto de falla (SPOF).
          p.w-75.mx-auto.textDc01 «Scale up»
      .col-md-6
        .p-5.Bg02
          h3 Escalamiento horizontal
          p.mb-4 Agrega nodos idénticos adicionales al servidor.
          h4.mb-4 Consideraciones:
          ol.lista-ol--cuadro.mb-4
            li 
              .lista-ol--cuadro__vineta
                span 1
              | Inversión adicional.
            li 
              .lista-ol--cuadro__vineta
                span 2
              p
                | Requiere 
                strong balanceo de carga 
                | para administrar la conexión.
          p.w-75.mx-auto.textDc01 «Scale out»
    
    #t1_5.titulo-segundo
      h2 1.5  Balanceo de carga
    
    p.mb-4 
      strong Distribución eficiente 
      | del 
      strong tráfico entrante 
      | a un sistema de software, a través de un grupo de componentes de software.
    
    .row.justify-content-center
      .col-md-10    
        figure
          img(src='@/assets/curso/img16.svg', alt='Alta disponibilidad')
  
</template>

<script>
export default {
  name: 'Tema1',
  components: {},
  data: () => ({
    // variables de vue
  }),
}
</script>

<style lang="sass" scoped></style>
