
##### 清除CURL缓存
- curl -vo /dev/null -X PURGE -H "[url]" -x [host]:[port]

##### CURL HTTP
- curl -vo /dev/null "[url]" -x [host]:[port]

##### CURL HTTPS
- curl -vo /dev/null "[url]" --resolve [domain]:[port]:[host]

##### CURL IPV6
- curl -vo /dev/null -s -6 "[url]" --resolve [domain]:[port]:[host]

##### CURL 增加头部
- curl -vo /dev/null -H "Range:bytes=0-512" "[url]" --resolve [domain]:[port]:[host]

##### CURL 设置返回格式
- curl -vo /dev/null -w "a=${a},b=${b}" "[url]" --resolve [domain]:[port]:[host]
