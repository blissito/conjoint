# JointsPro

## ¿Qué problema resuelve?

Imagina que necesitas lanzar un nuevo producto, pero no sabes qué características son realmente importantes para tus clientes. ¿Prefieren un precio bajo o más funcionalidades? ¿Les importa más la cámara o la batería?

**JointsPro** resuelve este problema mediante un análisis de preferencias que revela:

1. **Qué atributos son más importantes** para tus usuarios (ej: precio, tamaño, cámara)
2. **Cuánto vale cada característica** en la decisión de compra
3. **Cómo toman decisiones** los usuarios cuando evalúan opciones

## ¿Cómo funciona?

En lugar de preguntar directamente "¿qué es más importante para ti?", la herramienta:

1. Muestra diferentes opciones de productos con distintas combinaciones de características
2. Pide a los usuarios calificar su interés en cada opción (1-5)
3. Analiza estadísticamente las respuestas para descubrir las preferencias reales

## Los retos del análisis conjoint

El análisis conjoint es poderoso pero tiene desafíos importantes:

### 1. Diseño experimental
- Elegir qué atributos y niveles incluir no es trivial
- Demasiados atributos fatigan al participante
- Muy pocos atributos dejan información importante fuera
- Los niveles deben ser realistas y relevantes

### 2. Número de escenarios
- Un diseño factorial completo puede generar cientos de combinaciones
- Los participantes pierden atención después de ~15 evaluaciones
- Hay que balancear cobertura estadística vs. fatiga del usuario
- Diseños ortogonales reducen escenarios pero aumentan complejidad matemática

### 3. Interpretación de resultados
- Las utilidades son relativas, no absolutas
- Los resultados dependen de qué opciones se incluyeron
- Cambiar un nivel puede afectar la importancia de todo el resto
- No captura interacciones complejas entre atributos

### 4. Validez externa
- Las preferencias declaradas ≠ comportamiento real de compra
- El contexto de evaluación afecta las respuestas
- Sesgos cognitivos (anclaje, orden, etc.) pueden distorsionar resultados
- Lo que la gente dice que quiere no siempre es lo que termina comprando

### 5. Implementación técnica
- El análisis requiere regresión o modelos más sofisticados
- Los resultados a nivel individual son ruidosos
- Agregar muchos participantes puede ocultar segmentos importantes
- Balance entre simplicidad y rigor estadístico

## Demo

Abre `conjoint-example.html` en tu navegador para ver un ejemplo funcional. El demo usa un diseño simplificado con 12 escenarios y 4 atributos.

---

**Stack**: HTML + JavaScript vanilla (sin dependencias)
