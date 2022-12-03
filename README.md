# elasticsearch



f値で検索する
```sh
curl -XGET 'http://localhost:9200/image/_search' -d '{
  "query": {
    "range": {
      "f": {
        "gte": 0,
        "lte": 3.2
      }
    }
  }
}' -H "Content-Type: application/json"
```
