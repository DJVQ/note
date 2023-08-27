
##### 清除CURL缓存
- curl -vo /dev/null -X PURGE -H "[url]" -x [host]:[port]

##### CURL HTTP
- curl -vo /dev/null "[url]" -x [host]:[port]

##### CURL HTTPS
- curl -vo /dev/null "[url]" --resolve [domain]:[port]:[host]
