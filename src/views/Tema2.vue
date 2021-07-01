<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    .titulo-principal
      .titulo-principal__numero
        span 2
      h1 Balanceo de cargas con X-Road
    
    figure.mb-5
      img(src='@/assets/curso/img21.png', alt='Balanceo de carga con X-Road')
    
    #t2_1.titulo-segundo
      h2 2.1  Balanceo de carga interno
    
    p.mb-4
      | Característica incorporada de los 
      strong servidores de seguridad. 
      | El objetivo es la 
      strong alta disponibilidad.    
    
    .row.justify-content-around.mb-4
      .col-md-5
        hr.w-75.mx-auto
        .row.align-items-center
          .col-4.col-sm-3.col-lg-2.d-flex.align-items-center.bottom
            figure
              img(src='@/assets/curso/1.svg', alt='1')
          .col.py-3
            h3 Mecanismo integrado
            p
              strong X-Road 
              | tiene un mecanismo integrado para una 
              strong alta disponibilidad.
      .col-md-5
        hr.w-75.mx-auto
        .row.align-items-center
          .col-4.col-sm-3.col-lg-2.d-flex.align-items-center.bottom
            figure
              img(src='@/assets/curso/4.svg', alt='4')
          .col.py-3
            h3 Distribución de tráfico
            p 
              | Aunque no existe un algoritmo de balanceo de carga, el tráfico se distribuye entre los servidores de seguridad del proveedor según la 
              strong ubicación en la red.
      
      .col-md-5
        hr.w-75.mx-auto
        .row.align-items-center
          .col-4.col-sm-3.col-lg-2.d-flex.align-items-center.bottom
            figure
              img(src='@/assets/curso/2.svg', alt='2')
          .col.py-3
            h3 El más rápido
            p
              | Si la misma 
              strong organización, subsistema y servicio 
              | se han registrado en varios 
              strong servidores de seguridad, 
              | se utiliza el que responde 
              strong más rápido.
      .col-md-5
        hr.w-75.mx-auto
        .row.align-items-center
          .col-4.col-sm-3.col-lg-2.d-flex.align-items-center.bottom
            figure
              img(src='@/assets/curso/5.svg', alt='5')
          .col.py-3
            h3 Nuevos nodos
            p 
              | Agregar nuevos nodos significa configurar y registrar un nuevo 
              strong Servidor de Seguridad.
      
      .col-md-5
        hr.w-75.mx-auto
        .row.align-items-center
          .col-4.col-sm-3.col-lg-2.d-flex.align-items-center.bottom
            figure
              img(src='@/assets/curso/3.svg', alt='3')
          .col.py-3
            h3 Transparencia
            p
              | El 
              strong balanceo de carga interno 
              | es completamente transparente para el solicitante.
        hr.w-75.mx-auto

      .col-md-5
        hr.w-75.mx-auto
        .row.align-items-center
          .col-4.col-sm-3.col-lg-2.d-flex.align-items-center.bottom
            figure
              img(src='@/assets/curso/6.svg', alt='6')
          .col.py-3
            h3 Identidad
            p 
              | Cada nodo tiene su propia 
              strong identidad y certificados.
        hr.w-75.mx-auto
    
    .row.mb-4.justify-content-center
      .col-md-8.col-lg-4
        h4.ConTitle2 Balanceo de carga interno
    
    .row.justify-content-center.mb-5
      .col-md-10    
        figure
          img(src='@/assets/curso/img22.svg', alt='Balanceo de carga interno')
    
    #t2_2.titulo-segundo
      h2 2.2  Balanceo de carga externo
    
    p.mb-4
      | El objetivo es el 
      strong rendimiento.
    
    .row.mb-5
      .col-md-6.col-lg.tarjeta--tabla.p-4
        .row.justify-content-center.mb-3
          .col-4
            img(src='@/assets/curso/img23.svg' alt='AvatarTop')
        .h4.mb-4 Clúster
        ol.lista-ol
          li 
            span.text-bold 1. 
            p.mb-0
              strong Clúster 
              | con N nodos.
          li 
            span.text-bold 2. 
            p.mb-0
              | Todos los nodos están 
              strong activos 
              | y manejan el tráfico.

      .col-md-6.col-lg.tarjeta--tabla.p-4
        .row.justify-content-center.mb-3
          .col-4
            img(src='@/assets/curso/img24.svg' alt='AvatarTop')
        .h4.mb-4 Servidor de Seguridad y Balanceo
        ol.lista-ol
          li 
            span.text-bold 1. 
            p.mb-0
              | Los clientes ven el clúster como un 
              strong servidor de seguridad.
          li 
            span.text-bold 2. 
            p.mb-0
              | El 
              strong balanceador de carga 
              | (frente al clúster), distribuye las llamadas.

      .col-md-6.col-lg.tarjeta--tabla.p-4
        .row.justify-content-center.mb-3
          .col-4
            img(src='@/assets/curso/img25.svg' alt='AvatarTop')
        .h4.mb-4 Escalamiento Dinámico
        p.mb-0 
          | Como los nodos no tienen su propia identidad, el clúster se puede 
          strong escalar dinámicamente 
          | agregando / quitando nodos.

      .col-md-6.col-lg.tarjeta--tabla.p-4
        .row.justify-content-center.mb-3
          .col-4
            img(src='@/assets/curso/img26.svg' alt='AvatarTop')
        .h4.mb-4 Proceso de escalamiento
        p
          | El 
          strong proceso de escalamiento 
          | se puede basar, por ejemplo, en la carga de la CPU, el rendimiento de los mensajes o la programación predefinida.
    

    .row.mb-4.justify-content-center
      .col-md-8.col-lg-4
        h4.ConTitle2 Balanceo de carga externo
    
    .row.justify-content-center
      .col-md-10    
        figure
          img(src='@/assets/curso/img27.svg', alt='Balanceo de carga externo')


          
  
</template>

<script>
export default {
  name: 'Tema2',
  components: {},
  data: () => ({
    // variables de vue
  }),
}
</script>

<style lang="sass" scoped></style>
