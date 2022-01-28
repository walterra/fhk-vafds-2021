# Beispiele 20.11.2021

## Simple Workflow acquire/parse/filter/mine/represent/interact

Repository: https://github.com/walterra/miyo2elasticsearch

- Datentransformation mit `jq`, Datenvisualisierung mit Elasticsearch/Kibana<br/>
  [github.com/walterra/miyo2elasticsearch/blob/master/README.md](https://github.com/walterra/miyo2elasticsearch/blob/master/README.md)
- Datentransformation mit `pandas`, Datenvisualisierung mit `seaborn` und `shap`<br/>
  [github.com/walterra/miyo2elasticsearch/blob/master/miyo.ipynb](https://github.com/walterra/miyo2elasticsearch/blob/master/miyo.ipynb)
- Datenvisualisierung mit `altair`<br/>
  [github.com/walterra/miyo2elasticsearch/blob/master/miyo_altair.ipynb](https://github.com/walterra/miyo2elasticsearch/blob/master/miyo_altair.ipynb)

## Technology mix workflow

### COVID19 Web Scraping & Analyse Todesfälle

[github.com/walterra/covid-19-tirol-ds](https://github.com/walterra/covid-19-tirol-ds)

- acquire: `bash` scripts fuer web scraping
- parse/filter/mine: `nodejs` scripts
- analyse/visualize: `python/pandas/altair` notebooks
- deployment: `GitHub Actions`
- presentation: `altair` embedded in static `html/js` website

### COVID19 Analysis based on Open Data

[github.com/walterra/covid-19](https://github.com/walterra/covid-19)

- acquire: download CSV via `bash` scripts
- parse/filter/mine/analyse/visualize: `python/pandas/altair` notebooks
- deployment: `GitHub Actions`
- presentation: `altair` embedded in static `html/js` website

## Annotations

- Theme-Anpassung, Custom-Annotations, Auslagerung in Custom Function mit `seaborn`<br/>
  [github.com/walterra/fhk-vafds-2021/tree/main/seaborn_annotations](https://github.com/walterra/fhk-vafds-2021/tree/main/seaborn_annotations)

## Noteworthy Tools:

- `jq`, lightweight and flexible command-line JSON processor<br/>
  [stedolan.github.io/jq](https://stedolan.github.io/jq/)
- `seaborn`, statistical data visualization based on matplotlib<br/>
  [seaborn.pydata.org](https://seaborn.pydata.org/)
- `altair`, declarative statistical visualization library for Python, based on Vega and Vega-Lite<br/>
  [altair-viz.github.io](https://altair-viz.github.io/)
- `vega`, visualization grammar, a declarative language for creating, saving, and sharing interactive visualization designs<br/>
  [https://vega.github.io/vega](https://vega.github.io/vega/)
- Die `vega` web-runtime basiert auf `d3`, JavaScript library for producing dynamic, interactive data visualizations<br/>
  [d3js.org](https://d3js.org/)
- `Github Actions`<br/>
  [github.com/features/actions](https://github.com/features/actions)

