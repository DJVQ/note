#### 查看banben
- openssl version

#### 验证OCSP Stapling是否已经成功开启
- openssl s_client -connect [host]:[port] -status -tlsextdebug < /dev/null 2>&1 | grep -i "OCSP response"
