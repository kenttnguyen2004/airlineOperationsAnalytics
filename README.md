AIRLINE OPERATIONS ANALYTICS

An end-to-end data engineering and business intelligence project built with Python, PostgreSQL, and Tableau. It transforms public U.S. Bureau of Transportation Statistics (BTS) flight records into a validated dimensional model and an interactive dashboard for exploring on-time arrivals, arrival delays, cancellations, and diversions.

HOW IT WORKS
The current baseline profiles 539,747 January 2025 source records and analyzes a reproducible 50,000-flight sample. Python prepares and validates the data, PostgreSQL stores date, airline, and airport dimensions with a flight fact table, and a reporting CSV supplies Tableau. Source checksums, data-quality checks, and independent SQL/Python reconciliation connect dashboard results to the underlying data.

The Executive Overview includes six KPI cards, a daily on-time performance trend, and airline comparisons. Shared airline and date controls update the cards and charts together. The packaged Tableau workbook includes its CSV for local use without a running database.

INCLUDED IMAGES
1. executive-overview.png
   All airlines, January 1-31, 2025: 50,000 scheduled flights; 81.14% on-time arrivals among eligible flights; 3.04% cancellation rate.

2. first-week-overview.png
   All airlines, January 1-7, 2025: 11,759 scheduled flights; 72.94% on-time arrivals; 12.54 minutes average signed arrival delay.

3. filtered-aa-jan-01-07.png
   American Airlines (AA), January 1-7, 2025: 1,653 scheduled flights; 74.38% on-time arrivals; 16.71 minutes average signed arrival delay.

These are actual native Tableau dashboard PNG exports captured October 11, 2026, each at 2,200 x 1,700 pixels. The images are static; interactive controls are available in the workbook, which is not included in this image package.

METRIC DEFINITIONS AND SCOPE
On-time means arrival delay below 15 minutes among eligible flights. Arrival metrics exclude cancelled or diverted flights and missing arrival outcomes. Average arrival delay is signed, so early arrivals contribute negative minutes. Cancellation and diversion rates use all accepted scheduled records.

This is a locally verified January sample baseline, not a full-year build or a published dashboard. Sample comparisons are descriptive and do not establish causes or represent full-month population estimates. Full-year ingestion, dedicated airport/route/delay dashboards, automated refresh, and cloud deployment remain future work.
