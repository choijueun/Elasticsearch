# CRUD

## PUT

### INDEX 생성

    PUT (index명)

데이터 입력

> example

    $ curl -XPUT "http://localhost:9200/my_index/_doc/1" -H 'Content-Type: application/json' -d'
    {
    "name": "Jongmin Kim",
    "message": "안녕하세요 Elasticsearch"
    }'

> _CREATE

실수로 기존 도큐먼트가 덮어씌워지는 것을 방지

    6.x 이전 버전에서는 
    PUT <인덱스>/<도큐먼트 타입>/<도큐먼트 id>/_create