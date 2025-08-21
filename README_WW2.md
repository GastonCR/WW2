# WWII — Proyecto de Ciencia de Datos (OFFLINE, dataset incluido)

Este proyecto evita dependencias de red: incluye `data/ww2_country_panel.csv` con cifras reales **consolidadas** para 10 países principales.
Las cifras provienen de fuentes públicas (Wikipedia, Our World in Data, Maddison Project, páginas de producción por país) y se ofrecen como
**snapshot educativo** (los números exactos pueden diferir según la fuente).

## Contenido
- `notebooks/proyecto_WW2_offline.ipynb`: EDA + modelos (regresión/logística con LOOCV).
- `data/ww2_country_panel.csv`: dataset consolidado (bajas, población, PIB pc, aviones, tanques).
- `data/processed/ww2_country_panel_enriquecido.csv`: exportable con derivadas.
- `docs/Explicacion_WW2_OFFLINE.txt`: explicación breve del flujo.
- `requirements_ww2_offline.txt`: dependencias mínimas.

## Cómo ejecutar
```bash
pip install -r requirements_ww2_offline.txt
jupyter notebook notebooks/proyecto_WW2_offline.ipynb
```

## Notas
- **End-to-end**: desde dataset → EDA → modelos → métricas → exportables, todo sin internet.
- Podés reemplazar el CSV por otro más amplio (más países/variables) manteniendo los nombres de columnas.
