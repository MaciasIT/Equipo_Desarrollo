# 📝 Prompt para el Gerente de Producto

Este documento describe el propósito, la función y los componentes clave del prompt diseñado para el rol de Gerente de Producto en el desarrollo de aplicaciones impulsadas por IA.

## 🎯 Propósito y Función

El Prompt del Gerente de Producto es fundamental para transformar una idea inicial en un plan de producto estructurado y accionable. Imita el rol de un gerente de producto en una startup, ayudando a definir:

*   **Qué** se está construyendo.
*   **Por qué** se está construyendo (identificando el problema fundamental que la aplicación resolverá).
*   **Cómo** se medirá el éxito y si resuelve el problema para el usuario.

Este prompt instruye al modelo de IA a adoptar un enfoque de "problema primero", asegurando que todas las soluciones deriven de un problema central bien definido.

## 🔑 Componentes Clave que el Prompt Ayuda a Desarrollar

El prompt del Gerente de Producto facilita la generación de los siguientes entregables:

1.  **Personas de Usuario:** Descripciones detalladas de los usuarios objetivo.
2.  **Historias de Usuario Detalladas:** Narrativas que describen una funcionalidad desde la perspectiva del usuario.
3.  **Backlogs de Características:** Una lista priorizada de las funcionalidades a desarrollar.
4.  **Resumen Ejecutivo:**
    *   **"Elevator Pitch":** Una presentación concisa de una frase.
    *   **Declaración del Problema Central:** El problema principal que la aplicación busca resolver.
    *   **Audiencia Objetivo:** Descripción del segmento de usuarios al que se dirige la aplicación.
    *   **Diferenciación:** Qué hace que la solución sea única frente a las existentes.
    *   **Métricas de Éxito:** Cómo se medirá el impacto y el éxito de la solución.
5.  **Especificaciones Detalladas de Características:** Para cada característica, se define:
    *   Nombre de la característica.
    *   Historia de usuario principal (formato: "como un [usuario] quiero poder [acción] para poder [beneficio]").
    *   Problema central que resuelve.
    *   Requisitos funcionales (decisiones del usuario, gestión de estado, integraciones, etc.).
6.  **Requisitos Funcionales y Flujos de Trabajo del Usuario:** Descripción de cómo el usuario interactuará con la aplicación.
7.  **Requisitos Técnicos Iniciales:** Consideraciones iniciales sobre aspectos técnicos como gestión de estado, validación de datos, objetivos de rendimiento y uso de recursos.

## 🔗 Importancia en la Cadena de Prompts

Este prompt es vital porque, incluso antes de escribir una sola línea de código, proporciona una lista clara de requisitos iniciales y una comprensión profunda de la experiencia de usuario principal. El resultado de este prompt (los requisitos del Gerente de Producto) sirve como la entrada para el siguiente prompt esencial, el "Ingeniero de UX", quien traduce estas ideas en sistemas de diseño integrales y flujos de usuario detallados, asegurando una base de producto sólida y bien pensada desde el principio.