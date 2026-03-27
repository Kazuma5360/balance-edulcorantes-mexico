# balance-edulcorantes-mexico
Dashboard interactivo de oferta y demanda de edulcorantes en México 2011–2025 · Excel

**Autor:** [Kazuma5360](https://github.com/Kazuma5360)  
**Herramientas:** Excel (Tablas dinámicas, Segmentadores, Gráficas dinámicas) · Python (pandas, openpyxl)  
**Fuente de datos:** [SIAP — Servicio de Información Agroalimentaria y Pesquera](https://www.gob.mx/siap)

---

## 📌 Descripción del proyecto

Dashboard interactivo en Excel que analiza el balance mensual de oferta y demanda de edulcorantes en México entre 2011 y 2025, con foco en azúcar y jarabe de maíz rico en fructosa (JMRF).

El dashboard permite filtrar por concepto, año y mes mediante segmentadores dinámicos conectados a 4 visualizaciones y 4 KPIs que se actualizan en tiempo real.

---

## 📁 Estructura del archivo

```
balance_edulcorantes_portafolio.xlsx
│
├── Dashboard   → KPIs + 4 gráficas interactivas con segmentadores
├── Análisis    → Tabla comparativa Azúcar vs JMRF por año
└── Datos       → Dataset limpio (fuente: SIAP)
```

---

## 📈 Hallazgos principales

- **La producción de azúcar alcanzó su pico en 2013** (~6.5M toneladas) y ha caído sostenidamente desde entonces, llegando a 4.7M en 2025.
- **Las exportaciones colapsaron** — pasaron de 2.7M toneladas en 2013 a 759K en 2024, su nivel más bajo del período.
- **El consumo nacional se mantuvo estable** (~4M ton/año) a pesar de la caída en producción, sostenido por importaciones crecientes.
- **El JMRF es un producto importación-dependiente** — su producción local (~41,000 ton/mes) cubre menos del 30% del consumo nacional. El resto se importa, principalmente de Estados Unidos.
- **La balanza comercial acumulada** muestra que México exportó el 58.72% e importó el 41.28% del volumen total comercializado en el período.

---

## 🔁 Cómo reproducir el proyecto

### Opción A — Solo Excel
1. Descarga `balance_edulcorantes_portafolio.xlsx`
2. Abre en Excel 2016 o superior
3. Usa los segmentadores de **Concepto**, **Año** y **Mes** para explorar los datos

---

## 🗂️ Dataset

| Campo | Descripción |
|---|---|
| `año` / `mes` | Período del registro |
| `concepto` | `azucar` o `jmrf` |
| `produccion` | Producción nacional (toneladas) |
| `importaciones_totales` | Importaciones totales (toneladas) |
| `exportaciones_totales` | Exportaciones totales (toneladas) |
| `consumo_nacional_aparente` | Consumo nacional aparente (toneladas) |
| `inventario_final` | Stock al cierre del período (toneladas) |

**Registros:** 342 filas · 2 conceptos · 12 meses · 2011–2025  
**Nota:** `total_de_edulcorantes` fue excluido del análisis por ser una variable derivada.

## 📜 Licencia
Este proyecto está bajo la licencia [BSD 3-Clause](LICENSE). Siéntete libre de usarlo, modificarlo y distribuirlo, siempre que:

1. Se mantenga el aviso de copyright original
2. Se incluya la lista completa de condiciones
3. No se use el nombre de los contribuyentes para promocionar productos derivados sin permiso

Para más detalles, consulta el archivo [LICENSE](LICENSE).
