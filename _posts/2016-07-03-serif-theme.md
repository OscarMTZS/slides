---
title: "Unidad 2: Actuadores"
layout: post
permalink: /unidad-2-actuadores/
background: '#0a5'

slides:
  - title: "Unidad 2: Actuadores"
    slide-data: |
      Los actuadores son dispositivos que transforman energía en movimiento. Existen tres categorías principales:
      - Eléctricos: dependen de la electricidad para operar.
      - Mecánicos: funcionan a partir de piezas mecánicas.
      - Hidráulicos: utilizan fluidos presurizados.

  - title: "2.1 Actuadores Eléctricos"
    slide-data: "Estos actuadores emplean energía eléctrica para producir movimiento preciso y controlado."

  - title: "2.1.1 Tipos de Actuadores Eléctricos"
    slide-data: |
      - Motores de corriente directa (DC)
      - Motores paso a paso
      - Servomotores, que permiten un control preciso de posición y velocidad.

  - title: "2.1.2 Principio de Funcionamiento"
    slide-data: "Los actuadores eléctricos convierten la electricidad en energía mecánica, generando movimiento rotacional o lineal."

  - title: "2.1.3 Características de los Actuadores Eléctricos"
    slide-data: |
      - Alta precisión en el control del movimiento.
      - Capacidad para controlar tanto la velocidad como la posición de manera eficiente.

  - title: "2.1.4 Modos de Control"
    slide-data: |
      Los actuadores eléctricos pueden ser controlados mediante:
      - PWM (Modulación por Ancho de Pulso)
      - Comunicación serial para controles más complejos.

  - title: "2.2 Actuadores Mecánicos"
    slide-data: "Generan movimiento mediante la interacción directa entre componentes mecánicos."

  - title: "2.2.1 Tipos de Actuadores Mecánicos"
    slide-data: |
      - Engranajes
      - Poleas
      - Resortes, que almacenan energía para liberarla en forma de movimiento.

  - title: "2.2.2 Principio de Funcionamiento"
    slide-data: "Se basan en la interacción mecánica entre componentes para generar movimiento."

  - title: "2.2.3 Características de los Actuadores Mecánicos"
    slide-data: |
      - Generalmente económicos y duraderos.
      - Fiables para aplicaciones donde no se requiere alta precisión.

  - title: "2.2.4 Modos de Control"
    slide-data: "Funcionan de manera manual o automática, usando sistemas eléctricos simples."

  - title: "2.3 Actuadores Hidráulicos"
    slide-data: "Estos actuadores utilizan fluidos presurizados para generar movimiento lineal o rotatorio."

  - title: "2.3.1 Tipos de Actuadores Hidráulicos"
    slide-data: |
      - Cilindros hidráulicos: generan movimiento lineal.
      - Motores hidráulicos: producen movimiento rotacional.

  - title: "2.3.2 Principio de Funcionamiento"
    slide-data: "El fluido presurizado empuja un pistón dentro de un cilindro, lo que genera movimiento."

  - title: "2.3.3 Características de los Actuadores Hidráulicos"
    slide-data: |
      - Capaces de generar grandes fuerzas.
      - Menor precisión en comparación con actuadores eléctricos.

  - title: "2.3.4 Modos de Control"
    slide-data: "Controlados mediante válvulas que regulan el flujo y la presión del fluido."

  - title: "Fin de la Presentación"
    slide-data: "¡Gracias por su atención! Cualquier pregunta será atendida."
---
{% for slide in page.slides %}                 
<section data-background="{% if slide.image %}{{slide.image}}{% elsif slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}">
  <h1>{{slide.title}}</h1>
  <p>{{ slide.slide-data | markdownify }}</p>
</section>               
{% endfor %}



