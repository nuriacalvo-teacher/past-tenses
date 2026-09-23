# Past Tenses · EnglishPRO

App de práctica de los tiempos de pasado en inglés (ESO / Bachillerato), hecha con el mismo motor que [present-tenses](https://github.com/nuriacalvo-teacher/present-tenses).

**7 módulos × 3 niveles, con 10 ejercicios por nivel:**

1. Simple Past
2. Past Continuous
3. Past Perfect
4. Simple Past vs Present Perfect
5. Simple Past vs Past Continuous
6. Simple Past vs Past Perfect
7. Review of Past Tenses

- **Level 1:** opción múltiple (hace falta un 90 % para aprobar)
- **Level 2:** rellenar huecos (80 %)
- **Level 3:** traducción del español al inglés (80 %)

Cada módulo empieza con una explicación de uso con ejemplos. Los alumnos pueden entrar con su cuenta de Google y el código de clase, o como invitados (en ese caso no se guarda nada).

## Corrección de las traducciones

Se aceptan todas las respuestas correctas, no solo la del modelo:
- sinónimos (phone/mobile, mum/mother, film/movie, exam/test…)
- ortografía británica y americana (travelled/traveled, realised/realized…)
- contracciones (I'd = I had, didn't = did not…)
- el orden de las palabras y de las expresiones de tiempo
- otros tiempos verbales que también sean correctos en esa frase (por ejemplo, *after I finished* o *after I had finished*)
- *he* o *she* cuando la frase en español no lleva sujeto

Si hay que añadir una alternativa, se escribe en el campo `alts` de la frase. Dentro de una respuesta, `[a|b]` significa "vale a o b" y `[a|]` que la palabra es opcional.

## ⚠️ Firebase: hay que hacer una cosa una sola vez

Esta app guarda los resultados en su propio nodo, **`past_tenses_v1`** (el de present-tenses es `present_tenses_v2`), para que las notas de las dos apps no se mezclen.

En la consola de Firebase (proyecto *goya-english*): Realtime Database → **Reglas**. Duplica el bloque de `present_tenses_v2`, cambia el nombre a `past_tenses_v1` y publica.

Hasta que no lo hagas, el modo invitado funciona, pero la entrada con código de clase mostrará "Wrong class code".

## Publicarla

Settings → Pages → Deploy from a branch → `main` / root.
