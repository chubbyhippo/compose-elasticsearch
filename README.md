# elastic stack
## copy ca cert
```
docker cp compose-elasticsearch-elasticsearch-1:/usr/share/elasticsearch/config/certs/ca/ca.crt .
```
## test ca cert
```
curl --cacert ca.crt -u elastic:changeme https://localhost:9200
```