# Gantt Chart Maker

Paste a table, get a Gantt chart. Open it in a browser and it works, including offline.

**[Download](https://github.com/Data0000001/gant_maker/releases/latest/download/gantt-chart-maker.html)** — one HTML file, no install.

## How to use

- Download `gantt-chart-maker.html` and open it
- Paste data from a spreadsheet into the `Tasks` box
- Chart will be updated once data is changed
- Press `Update chart` if needed

## Data format
- One task per line, **tab-separated** (that's what you get when you copy from a spreadsheet)
- The **last two columns** are the start and end dates.
- **Everything before them** becomes its own label column to the left of the chart — however many you paste.
- A first row without dates is detected as a header and used for the column headings.
- If there are no tabs, two or more spaces are used as the separator instead.

Dates are read as `DD.MM.YYYY`, `DD/MM/YYYY`, `DD-MM-YYYY`, `YYYY-MM-DD`, and two-digit years. Slash format is day-first, not US month-first.

## What it does

- Export to PNG (`devicePixelRatio` aware).
- Column widths fit their content, capped by a slider so long text wraps instead of stretching the chart.
- Rows grow taller when a label wraps; bars and date labels stay centred.
- Month bands across the top, dashed marker on today's date.
