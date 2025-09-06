El Prompt de Arquitecto de Sistemas  
Propósito y Necesidad: Una vez que se tiene una comprensión clara de lo que hará la aplicación, gracias a los prompts de Product Manager y UX Engineer, la pregunta natural es "¿Cómo lo va a hacer?". El Prompt de Arquitecto de Sistemas ayuda a definir las elecciones y las compensaciones (trade-offs) técnicas que deben hacerse para cumplir con los requisitos del producto y el diseño. Es crucial para planificar cómo la aplicación manejará el crecimiento y los problemas de escala, por ejemplo, qué hacer si 500 usuarios intentan subir una imagen al mismo tiempo, para evitar que la aplicación falle. Este prompt aborda los requisitos de las características del producto para informar la arquitectura del sistema.  
Aspectos clave que considera este prompt: El prompt de Arquitecto de Sistemas está diseñado para detallar la infraestructura subyacente y las decisiones técnicas, incluyendo:  
• La arquitectura del sistema.  
• La infraestructura subyacente.  
• Cómo se modelarán e interconectarán los datos.  
• La estructura de la API.  
• Integraciones con servicios de terceros.  
• Consideraciones de seguridad y rendimiento.  
• Compensaciones (trade-offs) para el stack de front-end y back-end.  
• Elecciones de base de datos y almacenamiento.  
Proceso y Salida (Ejemplo con la aplicación Forkcast): Sean Kochel ilustra este prompt con el ejemplo de una segunda aplicación llamada Forkcast, una aplicación de cocina de acompañamiento impulsada por IA, que involucra procesamiento de imágenes, sistemas RAG (Retrieval Augmented Generation) agentivos, modelos de visión y chat de IA. Para Forkcast, se siguieron los mismos dos primeros pasos (Product Manager y UX Engineer), aunque con requisitos y pantallas de aplicación móvil mucho más robustos debido a la complejidad de la aplicación.  
La salida del prompt de Arquitecto de Sistemas para Forkcast incluyó un resumen ejecutivo de alto nivel que especificaba:  
• Front-end: Aplicación React Native con Expo.  
• Back-end: Fast API.  
• Base de datos: Supabase.  
• Procesamiento de IA: OpenAI.  
• Despliegue de la aplicación: Railway.  
• Límites técnicos: Procesamiento de imágenes de máximo 5 MB por foto, respuesta de IA con generación de recetas en 30-60 segundos, capacidad para manejar al menos 10,000 usuarios activos simultáneamente o en periodos de alta carga.  
También detalló el stack tecnológico para:  
• Front-end: React Native, Expo, Zustand para la gestión de estado, React Query para la gestión de consultas API, TypeScript.  
• Back-end: Python's Fast API, GraphQL, una capa Redis para caching y una cola Redis para procesar solicitudes de imágenes en lotes en segundo plano, permitiendo escalabilidad de recursos.  
Además, el prompt identificó los servicios externos a utilizar:  
• OpenAI: Para la API de visión, procesamiento general de recetas y generación de embeddings para características de IA.  
• Cloudinary: Para alojar imágenes.  
• Sentry: Para monitoreo y seguimiento de errores.  
La salida también proporcionó un plan de arquitectura de alto nivel que describe las interacciones entre los componentes, los servicios principales de la aplicación, las dependencias externas y las consideraciones para la integración con estos servicios (por ejemplo, qué se necesita para integrar con OpenAI o Cloudinary, y la importancia del tiempo de actividad de esos servicios). Se aborda la compatibilidad de las dependencias de front-end y back-end, y cómo se almacenará el estado del front-end (por ejemplo, un almacén de autenticación, un almacén de recetas, un almacén de perfil de usuario, un almacén de chat de IA).  
Beneficios y su Importancia para el "Vibe Coding": Este prompt es crucial porque permite que personas no ingenieras desplieguen soluciones significativas a problemas reales al proporcionar un plan técnico sólido. Ayuda a garantizar que la base de la aplicación esté bien establecida y evita que se tomen decisiones importantes sobre la marcha, que podrían depender del juicio de un modelo de lenguaje sin el contexto completo de la aplicación. Al pensar de antemano en patrones, convenciones y soluciones comunes a problemas que probablemente surgirán, se construye una base robusta