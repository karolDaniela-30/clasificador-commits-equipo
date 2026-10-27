# Informe tecnico: caracterizacion del modelo local

## 1. Perfil del equipo

- Sistema operativo: Ubuntu 24.04.5 LTS en WSL2.
- Memoria total visible en Ubuntu: 3.8 GiB.
- Memoria disponible antes de las pruebas: 3.3 GiB.
- Espacio de almacenamiento libre reportado anteriormente: aproximadamente 951 GB.

## 2. Modelo utilizado

- Nombre del modelo: gemma3:270m.
- Herramienta: Ollama.
- Tamano del modelo en disco: 291 MB.
- Prueba interactiva: el modelo respondio correctamente al saludo.
- Prueba de API REST: la solicitud fue exitosa y devolvio la respuesta "Hola".

## 3. Medicion de latencia

Se realizaron cinco solicitudes a la API de Ollama usando el mismo mensaje: "Responde solo con una palabra: hola".

| Prueba | Tiempo total |
|---|---:|
| 1 | 2.711 segundos |
| 2 | 2.467 segundos |
| 3 | 2.720 segundos |
| 4 | 2.953 segundos |
| 5 | 2.648 segundos |
| Promedio | 2.700 segundos |

El tiempo promedio de respuesta fue de aproximadamente 2.70 segundos por solicitud.

## 4. Memoria durante la inferencia

La memoria total visible en Ubuntu fue de 3.8 GiB y la memoria disponible antes de las pruebas fue de 3.3 GiB. No se obtuvo una medicion exacta de la RAM utilizada exclusivamente por el modelo durante la inferencia.

## 5. Calidad percibida

- Calificacion: 4 de 5.
- Observacion: el modelo respondio correctamente a las pruebas sencillas y genero respuestas comprensibles. Se debe probar con mensajes mas complejos para evaluar mejor su calidad.

## 6. Conclusion

El modelo gemma3:270m se instalo y funciono correctamente en Ollama. Se verifico su funcionamiento desde la terminal y mediante la API REST. En las cinco pruebas, el tiempo promedio de respuesta fue de aproximadamente 2.70 segundos. Estos resultados permiten continuar con las siguientes actividades del proyecto.
