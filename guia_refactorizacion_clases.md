# 🛠️ Guía Personal de Refactorización de Clases  
## Gestión por Líneas de Código

Esta guía documenta mi enfoque personal para mantener la **calidad** y la **manejabilidad** del código. Utilizo el número total de **líneas de código por archivo** como un indicador objetivo para decidir **cuándo y cómo refactorizar una clase**, evitando que crezca en tamaño y complejidad innecesariamente.

---

## 📌 Principios Fundamentales

### 🔹 Principio del Boy Scout  
> *"Deja el código un poco mejor de lo que lo encontraste."*  
Pequeñas mejoras continuas previenen problemas mayores.

### 🔹 Principio DRY (Don't Repeat Yourself)  
Evito la duplicación. La repetición indica la necesidad de abstraer o reorganizar.

### 🔹 Refactorización Continua  
No espero a que el código se vuelva inmanejable. Refactorizo como parte del flujo de trabajo.

---

## 📏 Umbrales de Líneas de Código y Acciones

### 🔸 Más de **150 líneas** – *Observación y Oportunidades Rápidas*
**Indicador:** La clase podría estar comenzando a crecer demasiado.  
**Acción principal:**  
- Evaluar el archivo rápidamente.
- Buscar **"victorias rápidas"** de bajo esfuerzo y alto impacto:

  ✅ Eliminar duplicación evidente  
  ✅ Extraer métodos pequeños  
  ✅ Renombrar para mejorar la claridad  
  ✅ Eliminar código muerto o comentarios obsoletos  

**Si no hay acciones inmediatas:**  
Agregar comentario `// TODO: Refactorizar – [Motivo breve]` como recordatorio para el futuro.

---

### 🔸 Más de **250 líneas** – *Análisis Detallado y Planificación Seria*
**Indicador:** Complejidad significativa.  
**Acción principal:**  
Análisis profundo de la clase, enfocándose en:

- ¿Viola el **Principio de Responsabilidad Única (SRP)**?  
- ¿Existen **code smells**? (métodos largos, muchos parámetros, dependencias acopladas)  
- ¿Se puede dividir en clases más pequeñas?  
- ¿Hay patrones de diseño aplicables?

**Resultado esperado:**  
Definir **una propuesta concreta de refactorización** (como tarea personal o TODO detallado) y estimar esfuerzo.

---

### 🔴 Más de **500 líneas** – *Bloqueo y Refactorización Obligatoria*
**Indicador:** Punto crítico de complejidad.  
**Acción principal:**

🚫 No se añade más código funcional a esta clase.  
🛠️ Se ejecuta el plan de refactorización definido. Si no existe, se crea inmediatamente.

**Objetivo:**  
Reducir significativamente el tamaño de la clase, idealmente por debajo de **250** o cerca de **150 líneas**.

**Requisito:**  
Ejecutar **pruebas unitarias e integración** rigurosas antes y después de la refactorización.

---

## 📐 Cómo Medir las Líneas de Código

- Utilizo el conteo total de líneas proporcionado por el **editor de texto o IDE**.
- Incluye **código, comentarios y líneas en blanco**.
- No es una métrica perfecta de complejidad, pero es **objetiva, rápida y consistente** para esta metodología.

---

## ✅ Beneficios de Esta Guía

- **Menor carga cognitiva:** decisiones claras y objetivas.
- **Mayor mantenibilidad:** clases pequeñas y enfocadas son más fáciles de entender, probar y modificar.
- **Prevención de problemas:** se detecta la complejidad antes de que se vuelva un obstáculo.
- **Mejora continua:** fomenta una cultura de código limpio y robusto a largo plazo.
