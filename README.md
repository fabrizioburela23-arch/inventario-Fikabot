# ⚽ Mundial 2026 · Predictor de Partidos

Aplicación web en **un solo archivo HTML** ([`index.html`](index.html)) para **entender y predecir** la
Copa Mundial de la FIFA 2026 (Canadá · México · Estados Unidos). Sin instalación, sin dependencias
externas: ábrela en cualquier navegador y funciona al instante, incluso sin conexión.

## ¿Qué hace?

- **⚔️ Partidos** — Los 72 choques de la fase de grupos, cada uno con su probabilidad de
  victoria / empate / derrota, el favorito y un marcador estimado. Búsqueda por selección y
  ordenación por "más parejos" o "más desnivelados".
- **🅰️ Grupos** — Los 12 grupos con su tabla esperada y la **probabilidad de cada selección de
  avanzar**, calculada con simulación Montecarlo. Marca los "grupos de la muerte".
- **🎯 Simulador** — Enfrenta a cualquier par de selecciones y obtén la predicción al instante,
  con opción de ventaja de local.
- **🏆 Predicción del torneo** — Simula el Mundial completo (grupos → eliminatorias) miles de
  veces para estimar **quién tiene más opciones de ser campeón**.
- **🏟️ Sedes y formato** — Las 16 sedes, el calendario de fechas clave y el nuevo formato de 48 equipos.
- **📊 Metodología** — Explicación clara y honesta del modelo y sus fuentes.

## El modelo

1. **Índice de poder** por selección, derivado del ranking FIFA (+ ventaja de local para los anfitriones).
2. **Motor Poisson/Elo**: la diferencia de índices se convierte en goles esperados; la distribución
   de Poisson da las probabilidades exactas de cada resultado.
3. **Simulación Montecarlo**: el torneo se juega miles de veces aplicando los criterios oficiales
   (puntos, diferencia de goles, mejores terceros) para estimar avance y título.

Las probabilidades son **estimaciones estadísticas**, no certezas: en el fútbol siempre manda el azar.

## Datos

Construido con datos reales del **sorteo oficial** (Washington D.C., 5 de diciembre de 2025) y del
ranking FIFA. Fuentes citadas dentro de la app (pestaña *Metodología*).

## Uso

Abre `index.html` en el navegador. También puede publicarse tal cual en GitHub Pages.

---
Hecho para **FIKA Group**.
