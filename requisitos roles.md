2.1. Agente 1: El Gerente de Producto (Product Manager)  
Este agente es fundamental para definir qué se está construyendo, por qué y cómo se medirá el éxito. Evita la creación de aplicaciones genéricas a partir de conceptos vagos ("Oye, quiero una aplicación de seguimiento del sueño, hazme una, por favor, adorable").

Ideas Clave y Funcionalidades:

Enfoque de "Problema Primero": El agente instruye al modelo a pensar a través del problema fundamental que el producto resolverá.  
Resumen Ejecutivo: Incluye el "elevator pitch," la declaración del problema principal, el público objetivo, la propuesta de valor única y las métricas de éxito.  
Especificaciones Detalladas de Funciones: Para cada función, se definen historias de usuario (ej. "Como \[rol\], quiero poder \[acción\] para poder \[beneficio\]") y requisitos funcionales detallados (estado, decisiones del usuario, integraciones).  
Ejemplo Práctico: Extensión de Chrome "Color IQ"

Problema Principal: Los compradores en línea gastan "toneladas de dinero en ropa que en realidad no les queda bien."  
Público Objetivo: Mujeres conscientes de la moda, de 25 a 45 años, que compran regularmente en línea.  
Funciones Clave (MVP inicial): Análisis de color en tiempo real (superposición instantánea de coincidencia de color), sistema de recomendación de color inteligente.  
Criterios de Aceptación: Ej. la coincidencia de color debe cargarse en dos segundos en una página de producto, manejar múltiples opciones de color, mostrar el porcentaje de coincidencia.  
2.2. Agente 2: El Ingeniero de UX (UX Engineer)  
Este agente se encarga de traducir las historias de usuario del gerente de producto en "sistemas de diseño integrales, flujos de usuario detallados y especificaciones listas para la implementación." Su objetivo es separar el diseño de la codificación para lograr un diseño superior.

Ideas Clave y Funcionalidades:

Filosofía de Diseño Cohesiva: Define principios como "simplicidad audaz," "espacio en blanco transpirable," y "teoría del color sistemática."  
Principios Centrales de UX: Considera el objetivo principal de cada pantalla, la mejor manera de presentar la información, y la revelación gradual de elementos para evitar la sobrecarga del usuario.  
Sistema de Diseño Integral: Crea tokens para desarrolladores (colores, tipografía, espaciado), define componentes compartidos y específicos de funciones, y especifica interacciones y estados de error.  
Documentación Robusta: Genera una documentación completa para que el modelo (y los desarrolladores) comprendan cómo utilizar los elementos de diseño.  
Ejemplo Práctico: Extensión de Chrome "Color IQ" (Continuación)

Maquetas y Especificaciones Visuales: Se generan maquetas para el análisis en tiempo real, incluyendo indicadores de porcentaje de coincidencia, estados de éxito (80-100% de coincidencia), estados de advertencia (60-80%), y estados de "no recomendado" (0-40%).  
Jerarquía Visual: Define la disposición de elementos como el porcentaje de coincidencia, el estado, el nombre del color, las recomendaciones y las acciones.  
Guía de Estilo Completa: Incluye colores primarios, secundarios, semánticos, de acento, tipografía, espaciado y componentes.  
2.3. Agente 3: El Arquitecto del Sistema (System Architect)  
Una vez que se comprende qué hará la aplicación, este agente se centra en cómo lo hará, abordando las opciones técnicas y las compensaciones para lograr las funciones planificadas.

Ideas Clave y Funcionalidades:

Planificación de Escalabilidad: Aborda escenarios como un aumento repentino de usuarios (ej. "qué vas a hacer cuando tu aplicación crezca repentinamente y ahora tengas 500 personas intentando subir una imagen exactamente al mismo tiempo").  
Definición de Arquitectura: Incluye la infraestructura subyacente, el modelado de datos, el diseño de API, la integración de servicios de terceros, la seguridad y el rendimiento.  
Consideraciones del Stack: Detalla las elecciones y las compensaciones para el frontend y el backend (ej. React Native con Expo, Fast API en Python), bases de datos (Superbase), almacenamiento (Cloudinary), servicios de IA (OpenAI), monitorización de errores (Sentry).  
Manejo de Cargas: Incorpora soluciones como Redis para caché y colas (Redis Queue) para procesar solicitudes en lotes durante picos de carga.  
Coherencia en la Toma de Decisiones: Asegura que las decisiones arquitectónicas importantes se tomen de antemano, no "sobre la marcha," garantizando una base sólida.  
Ejemplo Práctico: Aplicación de Cocina "Forkcast"

Resumen Ejecutivo: Aplicación React Native con Expo, backend Fast API, Superbase para la base de datos, OpenAI para el procesamiento de IA, despliegue en Railway.  
Requisitos de Rendimiento: Procesamiento de imágenes máx. 5 MB/foto, respuesta de IA en 30-60 segundos, capacidad para manejar 10.000 usuarios activos.  
Stack Tecnológico Detallado: Frontend (React Native, Expo, Zustand, React Query, TypeScript), Backend (Python Fast API, GraphQL, Redis layer, Redis Queue).  
Servicios Externos: OpenAI (API de visión, generación de recetas, embeddings), Cloudinary (alojamiento de imágenes), Sentry (monitorización de errores).  
Almacenamiento de Estado del Frontend: Autenticación, recetas, perfil de usuario, chat de IA.  
2.4. Agente 4: La Bola Demoledora (Wrecking Ball)  
Este agente actúa como un "especialista meticuloso en validación de requisitos." Su propósito es comparar lo que se pretendía construir inicialmente con lo que realmente se ha construido, identificando brechas y desviaciones.

Ideas Clave y Funcionalidades:

Conciliación de Requisitos: Compara los requisitos del Gerente de Producto y del Ingeniero de UX con la implementación real.  
Sistema de Validación de Tres Niveles:Requisitos: Identifica lo especificado pero no construido, y lo construido sin ser solicitado.  
Comportamiento Previsto: Evalúa la calidad de la implementación y si los recorridos de usuario se han completado correctamente.  
Resumen Ejecutivo y Desglose por Función: Proporciona una visión general y un análisis detallado de cada función.  
Ejemplo Práctico: "Forkcast" (Primera Versión MVP)

Resumen Ejecutivo: Se completó el 62% de los requisitos.  
Brechas Mayores Identificadas:Autenticación y Onboarding: Algunas cosas iniciadas pero no completadas.  
Captura de Fotos: 95% completa (falta detección de poca luz).  
Entrada del Menú: 90% completa (detección automática de cocina no incluida intencionalmente).  
Generación de Recetas: 70% completa (demasiado lento, falta sistema de notificación push, vista de receta podría tener más detalles).  
Historial y Gestión de Recetas: Muchas cosas incompletas (lista de recetas, vista detallada, edición básica, búsqueda/filtrado no implementado).  
Función de IA: No completada en esta fase.  
2.5. Agente 5: El Pulidor de UI (UI Polisher)  
Este agente ayuda a refinar la interfaz de usuario, evaluando el rendimiento actual contra las especificaciones de diseño originales y sugiriendo mejoras para lograr una apariencia "premium."

Ideas Clave y Funcionalidades:

Evaluación de Calidad del Diseño: Califica la implementación actual en comparación con las guías de UX/UI y los requisitos del producto.  
Identificación de Inconsistencias: Detecta áreas donde el sistema de diseño no se ha aplicado correctamente (ej. "el problema principal no es en realidad el sistema de diseño, es la implementación inconsistente y la falta de pulido en el sistema").  
Recomendaciones Específicas: Sugiere mejoras en áreas como sombras, gradientes, tipografía, flujo visual y microinteracciones.  
Proceso Iterativo: Permite retroalimentar las sugerencias a un agente de ingeniería frontend para implementar cambios y refinar el diseño.  
Ejemplo Práctico: "Forkcast" (Problemas de UI)

Diagnóstico: "La aplicación tiene bases técnicas sólidas pero se queda corta en la calidad del diseño que buscamos." Inconsistencias en la aplicación del sistema de diseño.  
Ejemplos de Problemas: La función de chat de IA se ve bien, pero la sección del libro de cocina tiene un sistema de diseño "completamente diferente," espaciado incorrecto, botones no utilizados en otro lugar, una sensación "aburrida."  
Mejoras Críticas Sugeridas: Aplicar el sistema de diseño correctamente, implementar sombras/gradientes/profundidad, completar pantallas, mejorar la tipografía y el flujo visual, añadir "pulido de sensación premium" (ej. microinteracciones).