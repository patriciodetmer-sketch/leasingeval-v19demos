# Leasit — Evaluación de Crédito Leasing

Agente de evaluación de riesgo de leasing tailored al mercado financiero chileno.

## Características

- ✅ Evaluación de riesgo de crédito leasing (CMF-aligned)
- ✅ Análisis financiero automático de empresas
- ✅ Scoring multipilar (Riesgo del Deudor, Riesgo del Activo, Riesgo Operacional)
- ✅ Cálculo de ratios financieros en tiempo real
- ✅ Exportación a PDF y Excel
- ✅ Interfaz dark-themed con sidebar y topbar
- ✅ Gestión de expedientes

## Stack

- **Frontend**: React 18.2 (CDN)
- **UI**: CSS vanilla + componentes React
- **Exportación**: jsPDF + XLSX
- **Almacenamiento**: localStorage (prototipo)

## Despliegue

Este es un sitio estático — solo necesita hospedaje HTTP.

### Vercel (Recomendado)

```bash
vercel deploy
```

### Desarrollo Local

```bash
python3 -m http.server 3000
# Abre http://localhost:3000
```

## Arquitectura

### Componentes React

- **Login** — Autenticación básica
- **Dashboard** — Vista resumida de expedientes
- **NuevaEval** — Formulario multi-paso para crear evaluaciones
- **Expedientes** — Listado y búsqueda de casos
- **DetalleExpediente** — Análisis completo con ratios y scoring
- **Layout** — Estructura sidebar + topbar

### Utilidades

- `calcScore()` — Cálculo de puntaje CMF
- `autoScores()` — Ratios financieros automáticos
- `exportPDF()` — Generación de reportes PDF
- `classify()` — Clasificación de riesgo (A, B, C, D)

## Regulación

La evaluación sigue directrices de:
- **CMF** (Comisión para el Mercado Financiero)
- **Ley 18.010** (Operaciones de leasing)
- **DICOM/SINACOFI** (Antecedentes crediticios)

## Próximos Pasos

- [ ] Persistencia en PostgreSQL
- [ ] Backend en FastAPI
- [ ] Integración con Claude API para análisis avanzado
- [ ] Módulo de alertas y notificaciones
- [ ] Dashboard analytics

## Licencia

Privado — Proyecto interno.

---

**Versión**: 1.0.0 (v19)  
**Último build**: 2026-04-14
