1\. El Prompt de Product Manager  
Contexto del "Vibe Coding" y el propósito de los prompts: Sean Kochel explica que el "vibe coding" a menudo tiene una "traición oculta": la implicación de que equivale a la irreflexión, llevando a problemas de seguridad o aplicaciones poco impresionantes. Sin embargo, él sostiene que el "vibe coding" significa construir sin la sintaxis del lenguaje, no sin pensar en lo que se está construyendo. Para superar la narrativa negativa y construir de manera efectiva, Kochel utiliza una docena de agentes o prompts diarios, destacando cinco como esenciales. Su objetivo en el canal es proporcionar una perspectiva práctica de lo que realmente funciona en la construcción y despliegue de flujos de trabajo y aplicaciones impulsadas por IA en negocios reales.  
Función y Proceso del Prompt de Product Manager: El Prompt de Product Manager es fundamental porque imita el rol de un gerente de producto en una startup, que ayuda a definir qué se está construyendo, por qué y cómo se sabrá si se ha construido con éxito y si resuelve el problema para el usuario. Su objetivo es transformar una idea cruda en un plan de producto estructurado y accionable.  
El prompt instruye al modelo de IA a pensar con un enfoque de "problema primero", identificando el problema fundamental que la aplicación resolverá, ya que todas las soluciones deben derivar de ese problema central. No se puede simplemente construir algo con un concepto vago como "Quiero una aplicación para rastrear el sueño" y esperar que la IA adivine la intención, ya que esto resultaría en una aplicación genérica y básica.  
Los componentes clave que este prompt ayuda a desarrollar incluyen:  
• Personas de usuario.  
• Historias de usuario detalladas.  
• Backlogs de características.  
• Un resumen ejecutivo, que abarca:  
    ◦ Un "elevator pitch" (presentación de una frase).  
    ◦ Una declaración del problema central.  
    ◦ La audiencia objetivo.  
    ◦ Lo que diferencia la solución de otras existentes.  
    ◦ Cómo se medirá el impacto del éxito.  
• Especificaciones detalladas de características: Para cada característica, se define su nombre, la historia de usuario principal ("como un \[usuario\] quiero poder \[acción\] para poder \[beneficio\]"), el problema central que resuelve y los requisitos funcionales (decisiones del usuario, gestión de estado, integraciones, etc.).  
Ejemplo de Aplicación: La extensión "Color IQ" Kochel ilustra el uso de este prompt con una aplicación llamada "Color IQ", una extensión de Chrome que ayuda a los usuarios a combinar piezas de ropa con su "estación de color" personal, un concepto de la moda basado en el color de cabello, piel y ojos.  
El prompt, utilizando un modelo como Claude Opus, genera una salida que incluye:  
• Elevator pitch y declaración del problema principal: Los compradores online gastan dinero en ropa que no les queda bien, y estas decisiones podrían evitarse con un sistema como Color IQ.  
• Audiencia objetivo: Mujeres conscientes de la moda, de 25 a 45 años, con ingresos específicos, que compran regularmente online y que pueden tener dificultades para combinar colores o entender por qué algunas prendas no les lucen.  
• Características y funcionalidades:  
    ◦ Un "overlay" en tiempo real que muestra una puntuación de coincidencia de color en la página del producto.  
    ◦ Criterios de aceptación para estas características, como el tiempo de carga del análisis de color (dentro de dos segundos).  
    ◦ Un sistema de recomendación de color inteligente.  
    ◦ Aunque el prompt inicialmente sugiere características como un cuestionario de incorporación o un "estilista personal", Kochel demuestra cómo se pueden eliminar o ajustar para enfocarse en un Producto Mínimo Viable (MVP) más contenido.  
• Requisitos funcionales y flujos de trabajo del usuario: Se detalla cómo un usuario interactuaría con la extensión, desde la activación automática en dominios compatibles hasta el análisis detallado y el guardado en una lista de deseos.  
• Requisitos técnicos iniciales: Se consideran aspectos como la gestión del estado, la validación de datos, los objetivos de rendimiento (velocidad de carga y análisis) y el uso de recursos del navegador.  
Importancia en la cadena de prompts: Este prompt es vital porque, incluso antes de escribir una sola línea de código, proporciona una lista clara de requisitos iniciales y una comprensión de la experiencia de usuario principal. Si no se toma el tiempo para definir esto, el modelo de lenguaje simplemente implementará lo que decida, sin alinearse necesariamente con la visión del constructor.  
El resultado de este prompt (los requisitos del Product Manager) sirve como la entrada para el siguiente prompt esencial, el "UX Engineer" (Ingeniero de Experiencia de Usuario), que se encarga de traducir estas ideas en sistemas de diseño integrales y flujos de usuario detallados. Esto asegura que la base del producto sea sólida y bien pensada desde el principio.