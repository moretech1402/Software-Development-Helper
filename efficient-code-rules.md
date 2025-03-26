# 🌟 Reglas Objetivas para Escribir y Refactorizar Código

Este documento contiene reglas objetivas que sigo para escribir y refactorizar código de manera eficiente y estructurada. Tener estas reglas me ayuda a ahorrar energía mental y mantener un código limpio, mantenible y fácil de entender.

---

## 🎯 Reglas Personales y de Uso Frecuente

1. **Si una línea de código ocupa más de 100 caracteres**, la divido en líneas más pequeñas.
2. **Si un método supera las 25 líneas (sin contar comentarios)**, lo simplifico.
3. **Si una clase supera las 100 líneas**, intento dividirla. Puede llegar hasta **500 líneas**, pero nunca más.
4. **Desarrollo solo la funcionalidad que necesito ahora**, sin preocuparme demasiado por el futuro.
5. **Aplico la estrategia del Boy Scout** → Siempre intento dejar el código mejor de como lo encontré.
6. **Si escribo algo dos veces, lo abstraigo inmediatamente**. Aunque lo recomendado es tres.
7. **Si un método recibe más de 3 parámetros**, intento agrupar algunos de ellos en un objeto.

---

## 📝 Reglas de Formato y Legibilidad

7. **No más de dos niveles de indentación por método**.
8. **Cada método debe hacer solo una cosa**.
9. **Los nombres de variables y métodos deben ser autoexplicativos**.
10. **Evitar comentarios explicativos cuando el código puede explicarse solo**.
11. **Prefiero `early return` sobre `else`**.

---

## 📦 Reglas de Organización del Código

12. **Cada archivo debe tener una única responsabilidad**.
13. **No más de tres parámetros en un método**.
14. **No mezclar lógica de negocio con lógica de presentación**.
15. **Evitar estados mutables innecesarios**.
16. **Las dependencias deben ser inyectadas, no instanciadas dentro de la clase**.

---

## 🏢 Reglas de Abstracción y Modularidad

17. **Si un bloque de código se repite en más de dos lugares, convertirlo en un método**.
18. **No crear clases o métodos abstractos “por si acaso”**.
19. **Las interfaces deben ser específicas, no genéricas**.
20. **El código debe depender de abstracciones, no implementaciones concretas**.

---

## 🔄 Reglas de Evolución y Mantenimiento

21. **No dejar código comentado en el repositorio**, ya existe en el control de versiones.
22. **Si una revisión de código requiere más de 15 minutos para entenderse, es muy grande**.
23. **Si un fragmento de código antiguo toma más de 10 minutos en entenderse, refactorizarlo**.
24. **Revisar si ya existe una dependencia antes de agregar una nueva**.
25. **No optimizar prematuramente**, si no es instantáneo.

---

## ✅ Reglas de Testing

26. **Cada bug encontrado debe tener su test que lo prevenga en el futuro**.
27. **Las pruebas deben ser rápidas y deterministas**.
28. **Probar el comportamiento, no la implementación**.
29. **Los tests unitarios deben ser independientes entre sí**.
30. **Seguir la pirámide de testing**. Más tests unitarios que de integración y más de integración que de UI.

---

## 🏃‍♂️ Reglas Personales para Mantener el Ritmo

31. **Si paso más de 30 minutos atascado en un problema, pido ayuda o cambio de tarea**.
32. **Hago commits pequeños y con descripciones claras**.
33. **Antes de agregar una librería nueva, reviso cuánto crecerán las dependencias**.
34. **Si no he usado una función en los últimos tres meses, reviso si realmente la necesito**.
35. **Cada vez que toco una parte del código, intento dejarla un poco mejor de lo que estaba**.
36. **Si una funcionalidad requiere más de una semana en desarrollarse, la divido en entregas más pequeñas**.

---

## 📚 Referencias y Estudios Relevantes

- **Principios SOLID** → [Ver más](https://www.webreactiva.com/cursos/masterclass/ejemplos-reales-de-refactorizacion-con-buenas-practicas?utm_source=chatgpt.com)
- **Complejidad ciclomática** → [Explicación en StackOverflow](https://es.stackoverflow.com/questions/1056/para-que-un-m%C3%A9todo-sea-%C3%B3ptimo-en-programaci%C3%B3n-orientada-a-objetos-debe-tener-un?utm_source=chatgpt.com)
- **Regla de Tres** → [Wikipedia](https://es.wikipedia.org/wiki/Regla_de_tres_%28programaci%C3%B3n_inform%C3%A1tica%29?utm_source=chatgpt.com)
- **Refactorización** → [Explicación en IONOS](https://www.ionos.com/es-us/digitalguide/paginas-web/desarrollo-web/que-es-la-refactorizacion/?utm_source=chatgpt.com)
- **Buenas prácticas de codificación** → [Artículo en Medium](https://medium.com/%40wibastidas/mejorando-tu-c%C3%B3digo-buenas-pr%C3%A1cticas-en-desarrollo-de-software-13e6b95e794c?utm_source=chatgpt.com)
- **Estrategias de refactorización** → [Computer Weekly](https://www.computerweekly.com/es/consejo/La-forma-correcta-e-incorrecta-de-pensar-en-la-refactorizacion-de-codigo?utm_source=chatgpt.com)
- **Principios TRUE de Sandi Metz** → [Wikipedia](https://es.wikipedia.org/wiki/Sandi_Metz?utm_source=chatgpt.com)

📌 **Reglas sujetas a evolución**: Conforme adquiero más experiencia, reviso y ajusto estas reglas según sea necesario.

