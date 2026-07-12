# Loto & Kino Stats

App de estadísticas y generador de combinaciones para Loto, Recargado, Revancha, Desquite y Kino (Chile).

- Historial de sorteos (`data.json`, actualizado automáticamente cada 12 horas por una tarea programada)
- Frecuencia de números (calientes / fríos)
- Generador de combinaciones: aleatorio, ponderado por frecuencia, ponderado por atraso, mixto, y un modo
  experimental de red neuronal (TensorFlow.js) que se reentrena solo con cada sorteo nuevo.

**Importante:** cada sorteo es un evento aleatorio e independiente. Ninguna combinación generada aquí tiene
más probabilidad real de ganar — esta app es solo para curiosidad y análisis estadístico, no una estrategia
de apuesta. Datos de origen no oficiales (chileresultados.com); verifica siempre en polla.cl.
