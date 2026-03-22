# Moodi APP

### Product Requirements Document

Status: In Progress | Version: 1.0 | Owner: Daniella

---

## 1. El Problema

Las plataformas de streaming funcionan por el historial, pero ellas no tienen la manera de saber como te sientes hoy, como fue tu día, que tipo de contenido quieres que te acompañe hoy, así que creamos moodi, esa compañera cinéfila que conoce muchas series, y además le importa como te sientes, tuviste un mal día, toma ve una comedia, estas almorzando en el break del trabajo, una serie light que no te haga pensar mientras te distraes, es viernes en la noche no tienes planes pero te hiciste pop corn, toma un drama para que te entrega.

**Contexto específico:**
Tienes 25 minutos para almorzar. El plato está caliente.
Abres Netflix y 10 minutos después todavía estás scrolleando.

---

## 2. Usuario Objetivo

- Tiene 2-4 suscripciones de streaming activas
- Consume series en todo momento y varias al tiempo
- Quiere recomendaciones que entiendan su estado de ánimo, su día, su entorno, su contexto.
- No tiene tiempo de ponerse a buscar entre todas sus suscripciones que puede ver hoy

---

## 3. Propuesta de Valor

Moodi es tu amiga cinéfila que se ha visto todo. Ha consumido una gran cantidad de serie, sabe que recomendarte según el contexto en el que estás actualmente, a veces queremos una serie que nos acompañe, algo que ver en este momento de tu vida. 

**No es un buscador. Es una amiga con criterio.**

---

## 4. Personalidad del Producto

- Tono: cercana, divertida, free, relajada
- Nunca dice: "Te recomiendo el siguiente contenido"
- Siempre dice: "Tengo lo que necesitas"
- Entiende contexto emocional y temporal
- Tiene opinión propia

---

## 5. Variables del Input

| Variable | Opciones |
| --- | --- |
| Mood | pesado / tranqui / feliz / ansioso / celebración |
| Tiempo | 20-30 min / 45 min / 1 hora / tarde libre |
| Momento | almuerzo entre semana / noche / finde |
| Plataformas | Netflix / HBO Max / Prime / Disney+/ Apple TV |

---

## 6. Las 3 Pantallas (MVP)

**Pantalla 1 — Input**

- Campo de texto libre: "¿Cómo estás hoy?"
- Selector de tiempo disponible
- Plataformas activas (configuradas en perfil)

**Pantalla 2 — Moodi piensa**

- Loading state con personalidad
- Mensajes tipo: "Te tengo algo que será perfecto para hoy..."

**Pantalla 3 — Output**

- 3 recomendaciones
- Por cada una: título, plataforma, duración,
por qué Moodi la eligió para ti hoy
- Link al trailer

---

## 7. Features MVP vs Futuro

### MVP ✅

- Input de mood en texto libre
- Recomendación de 3 opciones
- Filtro por plataforma
- Perfil con suscripciones activas

### V2 🔜

- Historial de lo que viste
- "No gracias, dame otra"
- Modo finde vs entre semana automático
- Ratings propios

### V3 💭

- Moodi aprende tus gustos con el tiempo
- Recomendaciones para ver en grupo
- Integración directa con plataformas

---

## 8. Pricing Model

| Plan | Precio | Qué incluye |
| --- | --- | --- |
| Free | $0 | 3 consultas por día |
| Moodi Pro | $4.99/mes | Ilimitado + historial + perfiles |

---

## 9. Métricas de Éxito

- Tiempo desde que abres Moodi hasta que pones algo: < 2 min
- % de recomendaciones que el usuario acepta: > 60%
- Retención semana 2: > 40%

---

## 10. Stack Técnico

- Frontend: Next.js + TypeScript + Tailwind
- AI: Claude API
- Deploy: Vercel
- Pagos: Stripe (V2)

---

## Log de Decisiones

| Fecha | Decisión | Por qué |
| --- | --- | --- |
| Hoy | MVP de 3 pantallas | Aprender el stack completo end-to-end |
| Hoy | Free tier con 3 consultas/día | Validar antes de monetizar |

---

## 11. User Stories

### Historia principal

**Como** usuaria con poco tiempo para almorzar,
**quiero** decirle a Moodi cómo me siento y cuánto tiempo tengo,
**para** empezar a ver algo en menos de 2 minutos sin frustrarme.

**Como** Usuaria es viernes, de una semana pesada, no tengo serie que ver 
**quiero** decirle a Moodi el tipo de serie que estoy buscando el ya sabe que plataformas tengo
**para** que me muestre tres recomendaciones en base a mis data, con lo que yo ya pago me lleve al trailer y pueda verla sin tener que buscar en toda la plataforma

**Como** usuario es un sábado en la noche, tengo los snacks listos queremos ver algo con mi pareja
**quiero** decirle a Moodi el tipo de película que quiero ver en el momento, el tipo de película que llegamos a un acuerdo los dos 
**para** que veamos tres recomendaciones y la capacidad de elegir se reduce y podemos disfrutar de los snacks más frescos 

### Historias secundarias

**Como** usuaria,
**quiero** configurar mis plataformas de streaming una sola vez,
**para** que Moodi solo me recomiende lo que puedo ver.

**Como** usuaria,
**quiero** que Moodi entienda si tengo 25 minutos o toda la tarde,
**para** recibir recomendaciones que se ajusten a mi tiempo real.

**Como** usuaria,
**quiero** saber por qué Moodi eligió esa recomendación para mí hoy,
**para** confiar en su criterio y no seguir dudando.

---

## 12. Winning Outcome

La usuaria abre Moodi, describe cómo se siente en una línea, y en menos de 2 minutos está viendo algo que le encanta, moodi aprende lo que le gusta ver cuando está triste, está contenta, cuando tuvo un día pesado, cuando quiere que la acompañen a almorzar.

**Éxito se ve así:**

- Cero scrolling en Plataformas después de usar Moodi
- La recomendación se siente como si una amiga la hubiera dado
- La usuaria vuelve mañana a la hora del almuerzo

---

## 13. Problem Outline

**Problema raíz:**
Los algoritmos de streaming optimizan para engagement a largo plazo,no para el momento específico en que estás, es imposible que ellos sepan como te sientes, la serie perfecta para ese día que abriste la plataforma.

**Por qué las soluciones actuales fallan:**

- Netflix recomienda basado en historial, no en mood
- Google "qué ver hoy" da listas genéricas sin contexto
- Preguntarle a amigos tarda demasiado
- Ninguna app combina mood + tiempo + plataformas disponibles

**El gap:**
No existe una herramienta que entienda: "Hoy tuve un día pesado, tengo 25 minutos, solo tengo Netflix y necesito algo que me haga reír."

---

## 14. Core Features (MVP)

### Must Have

- Input de texto libre con lenguaje natural
- Recomendación de 3 opciones con contexto
- Filtro automático por plataformas del usuario
- Explicación de por qué Moodi eligió cada opción
- Perfil con suscripciones activas
- Aprender y asociar el ánimo con las recomedaciones

### Should Have

- Selector visual de tiempo disponible
- "Dame otra opción" sin volver a empezar
- Loading state con personalidad de Moodi

### Nice to Have

- Historial de recomendaciones
- Rating después de ver
- Modo finde vs entre semana

### Never (fuera del scope)

- Reproducir contenido dentro de la app
- Ser otra plataforma de streaming
- Reemplazar el algoritmo de Netflix

---

## 15. UX Principles

**1. Velocidad sobre perfección**
Moodi debe dar una respuesta en segundos. El usuario no tiene tiempo — está almorzando.

**2. Personalidad antes que funcionalidad**
La forma en que Moodi habla ES el producto. Una recomendación genérica arruina la experiencia.

**3. Contexto lo es todo**
Sin mood + tiempo + plataforma = recomendación inútil.
El input debe ser tan fácil que no dé pereza hacerlo.

**4. Confianza a través de la explicación**
Moodi siempre dice por qué eligió algo. "Porque hoy tuviste un día pesado y esto te va a hacer reír sin que tengas que pensar mucho."

**5. Una decisión, no diez**
Máximo 3 opciones. Nunca más.
Más opciones = más parálisis = el problema original de nuevo.

1. **Moodi sabe quien es el usuario**

Moodi aprende el tipo de contenido al que recurre el usuario según su ánimo, así que sus recomendaciones son más personalizadas a partir del conocimiento

1. **Ya sabe que plataformas tengo** 

Moodi sabe que plataformas tiene y recomienda en esas, no en todas las posibles por que si no pago esa suscripción, no me interesa.