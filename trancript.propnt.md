# PROMPT: Formatear transcript de English Speaking Assessment a Markdown

## Contexto
Te voy a pasar el transcript en bruto de una práctica de speaking assessment de inglés que tuve con un bot evaluador. El texto viene revuelto, con timestamps, nombre del candidato repetido, frases cortadas, y las preguntas del bot mezcladas con mis respuestas en el mismo bloque de texto.

## Tu tarea
Reorganizar el transcript en un formato limpio de conversación entre dos personas (el bot evaluador y yo), listo para guardar en un archivo `.md`.

## Instrucciones específicas

### 1. Identificación de hablantes
- **Bot evaluador:** generalmente se presenta al inicio con un nombre (ej. Michael, Sarah, etc.). Hace preguntas, da feedback breve sobre mis respuestas, y transiciona entre temas.
- **Candidato (yo, Jesus):** doy respuestas más largas, a veces con muletillas ("so", "yeah"), frases incompletas o palabras repetidas porque hablo en tiempo real.

### 2. Limpieza del texto (importante)
- Elimina TODOS los timestamps (ej. "Jesus Uribe 0 minutes 58 seconds").
- Elimina las repeticiones del nombre del candidato que aparecen como separadores de bloques.
- Une fragmentos cortados que claramente pertenecen a la misma idea/oración.
- Corrige errores obvios de transcripción de voz a texto cuando el contexto lo deje claro (ej. "leave it run" → "go for a run", "turn off my AC" cuando el contexto dice que la prendió → "turn on my AC", "TE" → "IT", "Plaza" → "Pluralsight", "programmation" → "programming", "Buja" → muletilla a eliminar, etc.).
- Mantén el estilo natural de mis respuestas, pero hazlas legibles. NO inventes contenido nuevo, solo limpia lo que ya está.
- Conserva todas las ideas y ejemplos que mencioné, no resumas.

### 3. Formato Markdown
Usa exactamente esta estructura:

```markdown
# English Speaking Assessment - Practice Test

**Candidate:** Jesus Uribe
**Examiner:** [Nombre del bot]
**Duration:** ~[duración aproximada en minutos]

---

**[Nombre del bot]:** [intervención del bot]

**Jesus:** [mi respuesta]

---

**[Nombre del bot]:** [siguiente intervención del bot]

**Jesus:** [mi siguiente respuesta]

---
```

### 4. Reglas de formato (críticas para que el .md se vea bien)
- Negritas con `**` en los nombres de los hablantes.
- Línea separadora `---` entre cada intercambio (pregunta del bot + mi respuesta = un bloque).
- Línea en blanco entre el bloque del bot y mi bloque (sin `---` entre ellos, solo entre intercambios completos).
- Conserva el orden cronológico original de la conversación.
- Si el bot da feedback sobre mi respuesta anterior y luego hace una nueva pregunta, ambas cosas van juntas en su intervención.

### 5. Entrega
- Devuélveme el resultado dentro de un bloque de código markdown (con triple backtick) para que pueda copiarlo y pegarlo directamente en mi archivo `.md`.
- No agregues análisis ni feedback al final, solo el transcript formateado.
- Al final, en texto normal (fuera del bloque de código), pregúntame si quiero que analice mi nivel de inglés o si quiero algo más.

## Transcript a procesar
[AQUÍ PEGO EL TRANSCRIPT EN BRUTO]