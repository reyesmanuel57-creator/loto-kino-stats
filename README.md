# Estación Meteorológica Chile + Loto & Kino Stats

App web con dos secciones:

## 🌦️ Clima (principal)
Estación meteorológica con datos de las 16 capitales regionales de Chile, usando
[Open-Meteo](https://open-meteo.com) (gratuito, sin API key):

- Clima actual por región (`weather_data.json`, actualizado automáticamente cada 30 minutos)
- Pronóstico oficial a 7 días
- Pronóstico propio: modelo de tendencia (regresión lineal amortiguada) calculado sobre el
  historial diario que la app va acumulando — mejora con el tiempo
- Mapa con marcadores por región y capa de precipitación en vivo (RainViewer)
- Histórico diario e intradiario (últimas 48 h) por región

## 🎲 Loto & Kino Stats
App de estadísticas y generador de combinaciones para Loto, Recargado, Revancha, Desquite y Kino (Chile).

- Historial de sorteos (`data.json`, actualizado automáticamente cada 12 horas por una tarea programada)
- Frecuencia de números (calientes / fríos)
- Generador de combinaciones: aleatorio, ponderado por frecuencia, ponderado por atraso, mixto, y un modo
  experimental de red neuronal (TensorFlow.js) que se reentrena solo con cada sorteo nuevo.

**Importante:** cada sorteo es un evento aleatorio e independiente. Ninguna combinación generada aquí tiene
más probabilidad real de ganar — esta app es solo para curiosidad y análisis estadístico, no una estrategia
de apuesta. Datos de origen no oficiales (chileresultados.com); verifica siempre en polla.cl.

Los datos de clima tampoco son oficiales — para pronósticos oficiales usa la Dirección Meteorológica de Chile
(meteochile.gob.cl).
