# CRUD

## PUT

> example

    $ curl -XPUT "http://localhost:9200/my_index/_doc/1" -H 'Content-Type: application/json' -d'
    {
    "name": "Jongmin Kim",
    "message": "안녕하세요 Elasticsearch"
    }'

