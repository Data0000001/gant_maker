# Gantt Chart Maker

Paste a table, get a Gantt chart. Open it in a browser and it works, including offline.

## How to use

Download `Gant Chart Maker.html` and open it

## Data format

One task per line, tab-separated (that's what you get when you copy from a spreadsheet):

- The **last two columns** are the start and end dates.
- **Everything before them** becomes its own label column to the left of the chart — however many you paste.
- A first row without dates is detected as a header and used for the column headings.
- If there are no tabs, two or more spaces are used as the separator instead.

Dates are read as `DD.MM.YYYY`, `DD/MM/YYYY`, `DD-MM-YYYY`, `YYYY-MM-DD`, and two-digit years. Slash format is day-first, not US month-first.

## What it does

- Export to PNG (`devicePixelRatio` aware).
- Column widths fit their content, capped by a slider so long text wraps instead of stretching the chart.
