# 📝 Prompt para el Arquitecto de Sistemas

Este documento describe el propósito, la función y los componentes clave del prompt diseñado para el rol de Arquitecto de Sistemas en el desarrollo de aplicaciones impulsadas por IA.

## 🎯 Propósito y Función

El "Prompt de Arquitecto de Sistemas" ayuda a definir las elecciones y las compensaciones técnicas necesarias para implementar las características de la aplicación. Responde a la pregunta fundamental de "¿Cómo funcionará la aplicación?" una vez que se tiene una comprensión clara de "qué" hará (definido por el Gerente de Producto) y "cómo se verá y sentirá" (definido por el Ingeniero de UX).

Es crucial para planificar la infraestructura subyacente, el modelado de datos, las APIs, las integraciones con servicios de terceros, la seguridad y el rendimiento, previendo el escalado y las cargas de usuarios.

## 💡 Beneficios Clave

Este prompt es crucial porque permite que personas no ingenieras desplieguen soluciones significativas a problemas reales al proporcionar un plan técnico sólido. Ayuda a garantizar que la base de la aplicación esté bien establecida y evita que se tomen decisiones importantes sobre la marcha, que podrían depender del juicio de un modelo de lenguaje sin el contexto completo de la aplicación. Al pensar de antemano en patrones, convenciones y soluciones comunes a problemas que probablemente surgirán, se construye una base robusta.

## 🔑 Componentes Clave que el Prompt Ayuda a Desarrollar

El prompt del Arquitecto de Sistemas está diseñado para detallar la infraestructura subyacente y las decisiones técnicas, incluyendo:

1.  **Arquitectura del Sistema:** Definición de la estructura general de la aplicación.
2.  **Infraestructura Subyacente:** Componentes de hardware y software necesarios.
3.  **Modelado de Datos:** Cómo se estructurarán y interconectarán los datos.
4.  **Estructura de la API:** Diseño de las interfaces de programación de aplicaciones.
5.  **Integraciones con Servicios de Terceros:** Conexiones con plataformas y servicios externos.
6.  **Consideraciones de Seguridad y Rendimiento:** Estrategias para proteger la aplicación y asegurar su eficiencia.
7.  **Compensaciones (Trade-offs) para el Stack de Front-end y Back-end:** Decisiones sobre tecnologías y sus implicaciones.
8.  **Elecciones de Base de Datos y Almacenamiento:** Selección de sistemas de gestión de bases de datos y soluciones de almacenamiento.
9.  **Resumen Ejecutivo de Alto Nivel:** Incluye la pila tecnológica (front-end, back-end, base de datos, procesamiento de IA, despliegue) y límites técnicos (ej. procesamiento de imágenes, tiempo de respuesta de IA, capacidad de usuarios activos).
10. **Stack Tecnológico Detallado:** Especificaciones de las tecnologías a utilizar (ej. React Native, Expo, Zustand, React Query, TypeScript para front-end; Python's Fast API, GraphQL, Redis para back-end).
11. **Servicios Externos:** Identificación de servicios como OpenAI (visión, embeddings), Cloudinary (alojamiento de imágenes) y Sentry (monitoreo de errores).
12. **Plan de Arquitectura de Alto Nivel:** Describe las interacciones entre componentes, servicios principales, dependencias externas y consideraciones de integración.
13. **Almacenamiento de Estado del Front-end:** Cómo se gestionará el estado de la aplicación en el lado del cliente (ej. autenticación, recetas, perfil de usuario, chat de IA).

## 🔗 Conexión con los Siguientes Pasos

La salida del "Prompt de Arquitecto de Sistemas" proporciona la base técnica para la implementación y es crucial para los siguientes prompts en la cadena de desarrollo:

*   **Prompt de Bola de Demolición:** Para validar la implementación contra los requisitos técnicos y funcionales.
*   **Prompt de Pulidor de UI:** Aunque no directamente, las decisiones arquitectónicas pueden influir en la capacidad de implementar ciertos aspectos de pulido de UI.

Este prompt asegura que la construcción rápida con IA esté fundamentada en una base técnica sólida y escalable.