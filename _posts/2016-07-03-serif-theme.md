title: "Unidad 2: Actuadores"
layout: post
permalink: /unidad-2-actuadores/
background: '#0a5'

slides:

title: "Unidad 2: Actuadores" slide-data: | Los actuadores transforman distintas formas de energía en movimiento mecánico. Generalmente se dividen en tres grandes grupos:

Actuadores Eléctricos
Actuadores Mecánicos
Actuadores Hidráulicos
title: "2.1 Eléctricos" slide-data: "Estos actuadores emplean corriente eléctrica para generar desplazamientos o movimientos en diferentes sistemas."

title: "2.1.1 Tipos" slide-data: |

Motores de corriente continua (DC)
Motores de pasos
Servomotores
title: "2.1.2 Funcionamiento" slide-data: "Transforman la energía eléctrica en movimiento mecánico a través de mecanismos internos."

title: "2.1.3 Características" slide-data: |

Gran precisión
Posibilidad de controlar tanto la velocidad como la posición
title: "2.1.4 Modo de comunicación" slide-data: |

Modulación de ancho de pulso (PWM)
Comunicación mediante puertos seriales
title: "2.2 Mecánicos" slide-data: "Los actuadores mecánicos generan movimiento a través de la interacción directa entre piezas o mecanismos físicos."

title: "2.2.1 Tipos" slide-data: |

Sistemas de engranajes
Mecanismos de resortes
Poleas y correas
title: "2.2.2 Funcionamiento" slide-data: "El movimiento ocurre por la acción de componentes mecánicos que interactúan entre sí."

title: "2.2.3 Características" slide-data: |

Bajo costo en comparación con otros tipos
Fiabilidad en operaciones simples
title: "2.2.4 Modo de comunicación" slide-data: "Pueden ser activados manualmente o a través de dispositivos eléctricos sencillos."

title: "2.3 Hidráulicos" slide-data: "Utilizan fluidos presurizados para crear movimientos o aplicar fuerza."

title: "2.3.1 Tipos" slide-data: |

Pistones hidráulicos
Motores de fluido
title: "2.3.2 Funcionamiento" slide-data: "El fluido presurizado genera movimiento, normalmente impulsando un émbolo o creando rotación."

title: "2.3.3 Características" slide-data: |

Capaces de generar grandes fuerzas
No tan precisos como otros actuadores
title: "2.3.4 Modo de comunicación" slide-data: |

Control mediante válvulas y reguladores de flujo
title: "Fin de la Presentación" slide-data: "¡Gracias por su atención!"

{% for slide in page.slides %}                 
<section data-background="{% if slide.image %}{{slide.image}}{% elsif slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}">
  <h1>{{slide.title}}</h1>
  <p>{{ slide.slide-data | markdownify }}</p>
</section>               
{% endfor %}


