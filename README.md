# Calidad del Software
# Autor: Francisco Higuera

Repositorio de apoyo para la materia **Calidad del Software**. Reúne conceptos fundamentales y sirve como espacio para ejercicios, prácticas y evidencias relacionadas con la calidad y las pruebas de software.

## Conceptos básicos

- **Calidad del software:** grado en que un producto cumple los requisitos y satisface las necesidades de sus usuarios, considerando aspectos como funcionalidad, confiabilidad, seguridad, eficiencia y facilidad de mantenimiento.
- **Aseguramiento de la calidad (QA):** actividades planificadas para prevenir defectos y mejorar los procesos de desarrollo.
- **Control de calidad (QC):** actividades de revisión y pruebas para detectar defectos en el producto.
- **Verificación:** comprobar que el producto se construye de acuerdo con las especificaciones: «¿lo estamos construyendo correctamente?».
- **Validación:** comprobar que el producto resuelve las necesidades reales de sus usuarios: «¿estamos construyendo lo correcto?».
- **Defecto:** imperfección en un artefacto; puede provocar un **error** durante la ejecución y, eventualmente, una **falla** observable para el usuario.

## Pruebas de software

Las pruebas ayudan a evaluar el comportamiento del software, detectar defectos y aportar información para tomar decisiones. Deben planificarse según el riesgo y los requisitos; no garantizan por sí solas que el sistema esté libre de defectos.

### Tests unitarios

Comprueban una unidad pequeña y aislada —por ejemplo, una función o método— de forma rápida y repetible. Normalmente usan datos controlados y reemplazan dependencias externas cuando es necesario.

**Ejemplo:** probar que una función que calcula el total de una compra aplique correctamente un descuento. Un test unitario debería verificar tanto el resultado esperado como casos límite relevantes.

### Pruebas de integración

Comprueban que varios módulos o servicios funcionen correctamente en conjunto, por ejemplo, la interacción entre una aplicación y una base de datos.

### Pruebas end-to-end (E2E)

Comprueban un flujo completo desde la perspectiva de una persona usuaria, recorriendo los componentes principales del sistema —como la interfaz, el servidor y la persistencia—. Por ejemplo: iniciar sesión, crear un registro y confirmar que aparece en la lista.

Las pruebas E2E aportan confianza en los flujos críticos, pero suelen ser más lentas y sensibles a cambios en el entorno que los tests unitarios. Conviene mantenerlas enfocadas en los recorridos importantes.

## Pirámide de pruebas

Una estrategia equilibrada suele incluir muchos tests unitarios, pruebas de integración para interacciones relevantes y un conjunto acotado de pruebas E2E para los flujos críticos. La proporción depende del sistema y de sus riesgos.

| Nivel | Alcance | Velocidad habitual |
| --- | --- | --- |
| Unitario | Una función, método o unidad aislada | Alta |
| Integración | Interacción entre componentes | Media |
| E2E | Flujo completo del sistema | Menor |

## Buenas prácticas

- Relacionar las pruebas con requisitos, historias de usuario y riesgos.
- Usar nombres claros que describan el escenario y el resultado esperado.
- Mantener las pruebas independientes, deterministas y fáciles de ejecutar.
- Incluir casos normales, límites y entradas inválidas relevantes.
- Evitar que una prueba dependa del orden o del resultado de otra.
- Revisar los fallos y mantener las pruebas junto con el código.
- Tratar la cobertura como una señal útil, no como garantía de calidad.

## Organización del repositorio

Este README presenta la base conceptual del repositorio. A medida que se agreguen prácticas, se recomienda documentar para cada una su objetivo, requisitos, pasos para ejecutarla y resultados obtenidos. Las herramientas y comandos de prueba dependerán de la configuración concreta de cada proyecto.
