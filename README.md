# Z-Score Monitor — Pruebas de Rendimiento

Aplicación web interactiva para calcular el z-score de múltiples pruebas de rendimiento en tiempo real. Sin instalación, sin servidor — abre y funciona.

## Pruebas disponibles

| Prueba | Unidad | Uso típico |
|--------|--------|------------|
| Altura CMJ | cm | Potencia de salto |
| Peak Force IMTP | N | Fuerza máxima isométrica |
| Peak Force CMJ | N | Pico de fuerza en salto |
| Impulso Propulsivo CMJ | N·s | Capacidad propulsiva |
| RSI | m/s | Índice de fuerza reactiva |
| RFD Máx | N/s | Tasa de desarrollo de fuerza |

## Funcionalidades

- **Calculadora interactiva** con sliders por prueba
- **Registro de sesiones** por atleta (guardado en localStorage)
- **Cálculo automático** de media, SD y z-score cuando hay ≥10 sesiones
- **Exportar CSV** de todos los registros
- **Educación integrada**: comparación entre atletas y rol de la SD

## ¿Cómo usarla?

Abre directamente: **https://TU-USUARIO.github.io/zscore-cmj-calculator/**

## Umbrales

| z-score | Clasificación | Acción |
|---------|--------------|--------|
| ≥ +0.5 | Positivo | Buen día, estímulos de calidad |
| −0.5 a +0.5 | Normal | Seguir programa |
| −0.5 a −1.0 | Leve | Preguntar sensaciones |
| −1.0 a −2.0 | Alerta | Reducir carga |
| < −2.0 | Alerta alta | Revisar fatiga/salud |

## Recomendación

Necesitas al menos **10 sesiones registradas** para que la media y SD sean estadísticamente fiables. Antes de eso, el z-score es orientativo.

## Despliegue

1. Crea un repositorio en GitHub
2. Sube `index.html` y `README.md`
3. Settings → Pages → Source: **main branch** → Save
4. Listo en `https://tu-usuario.github.io/nombre-repo/`

## Privacidad

Todos los datos se guardan en tu navegador (localStorage). Nada se envía a ningún servidor.

## Licencia

MIT
