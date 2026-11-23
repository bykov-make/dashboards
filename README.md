# Power BI Dashboards

A collection of Power BI dashboards built to turn operational data into decisions.

## Customer Service Tracking (dashboard-ATC)

**Seguimiento de Servicios – Atención al Cliente**

## Business question

How is the customer service team performing, and where should a supervisor focus? The dashboard gives a one-page view of call volume, resolution, response speed, and customer satisfaction, filterable by period.

### Data

`Datos_de _servicio.xlsx`, sheet `atenciones`: 1,009 customer service calls from March 2023. This is a sample practice dataset, not real company data.

| Field | Description |
|---|---|
| Id Llamada | Call ID |
| Fecha | Call date |
| Asistente | Agent who handled the call (7 agents) |
| Área | Service area: Sales, Cancellations, Exchanges, Complaints |
| Respondido - Resuelto (S/N) | Whether the call was answered and resolved |
| Velocidad de respuesta | Time to answer, in seconds |
| Duración con asistente en segundos | Time spent with the agent, in seconds |
| Índice de satisfacción | Customer satisfaction score (1–5) |

The workbook also includes an `i18n` sheet with English/Spanish labels for every dashboard element, prepared for a bilingual version of the report.

### What the dashboard shows
- **Total calls**, **average satisfaction**, and **average wait time** as KPI cards
- **Resolution status**: share of calls resolved vs. not resolved (donut chart)
- **Calls per agent** (bar chart)
- **Calls by service area** (treemap)
- **Calls by date**, with drill-down by year, quarter, month, and day
- **Period filter** (date slicer)

### Key insights from the data
- **92.7%** of calls were resolved (935 of 1,009).
- **Sales** resolved 100% of its calls, while **Cancellations** had the lowest resolution rate (85.1%), which makes it the first area to review.
- **Average satisfaction is 3.4 / 5** and is almost identical across areas (3.38–3.44), so low satisfaction is not driven by one specific area.
- Average **wait time is 67 seconds**, and the average call lasts **3 min 44 s** with the agent.
- **Sales** represents 41% of all calls (411).

### Design

Custom background designed for the report, with a dark theme and color-coded KPI cards for quick reading.

### Tools

Power BI Desktop, Power Query, Excel.

### Screenshot

<img width="1423" height="803" alt="dashboard_atc" src="https://github.com/user-attachments/assets/2a627178-e69f-4944-97d4-4d83143f04b8" />

### How to open

Download dashboard-ATC/AtencionAlCliente.pbix and open it in Power BI Desktop. The data source is Datos_de _servicio.xlsx in the same folder; if prompted, update the file path under Transform data → Data source settings.
