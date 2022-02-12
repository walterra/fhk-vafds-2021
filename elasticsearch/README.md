## Elasticsearch / Kibana / eland

## Resources

- Download Elasticsearch: https://www.elastic.co/downloads/elasticsearch
- Download Kibana: https://www.elastic.co/downloads/kibana
- Eland: https://github.com/elastic/eland
- Jupyter / eland / Kibana / Vega https://github.com/walterra/jupyter2kibana
- Eland / Altair https://github.com/walterra/python-viz/tree/master/eland
- Custom Dashboard: https://www.elastic.co/blog/understanding-evolution-volcano-eruption-elastic-maps?ultron=community&blade=twitter&hulk=social&linkId=148912543

## Example Queries

```
# Alle Indices auflisten
GET _cat/indices

# Standard Suche
GET farequote_eland_2/_search

## Terms Aggregation, liefert Top 20 Airlines + Count
GET farequote_eland_2/_search
{
  "aggs": {
    "status_code": {
      "terms": { "field": "airline", "size":20 }
    }
  },
  "size":0
}

## Average Aggregation
GET farequote_eland_2/_search
{
  "aggs": {
    "responsetime_avg": {
      "avg": { "field": "responsetime" }
    }
  },
  "size":0
}


## date_histogram Aggregation fuer Time Series data
GET farequote_eland_2/_search
{
  "aggs": {
    "timeseries": {
      "date_histogram": { "field": "time", "calendar_interval": "1m"
      }
    }
  },
  "size":0
}

## Nested Aggregation fuer metrikbasierte Time Series
GET farequote_eland_2/_search
{
  "aggs": {
    "timeseries": {
      "date_histogram": { "field": "time", "calendar_interval": "1m"
      },
      "aggs": {
        "responsetime_stats": {
          "stats": { "field": "responsetime" }
        }
      }
    }
  },
  "size":0
}
```



