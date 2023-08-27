#### add service
- firewall-cmd --permanent --new-service="[service name]"
- firewall-cmd --permanent --service="[service name]" --set-short="[service short]"
- firewall-cmd --permanent --service="[service name]" --set-description="[service description]"
- firewall-cmd --permanent --service="[service name]" --add-port="[port]/[protocol]"

#### add public zone and rich rule
- firewall-cmd --permanent --zone=public --set-short="[zone name default is public]"
- firewall-cmd --permanent --zone=public --add-service="[service name]"
- firewall-cmd --permanent --add-rich-rule="rule family="[ipv4/ipv6]" source address="[source host]/[source port]" service name="[service name]" [tactics:accept|reject|drop]"

#### add direct rule
- firewall-cmd --permanent --direct --add-rule [ipv4/ipv6] [raw|manage|nat|filter] [PREROUTING|POSTROUTING|INPUT|OUTPUT|FORWARD] [permission level:0、1...] --destination [host] --protocol [vrrp] -j [ACCEPT|DROP|REJECT|LOG|NOTRACK|DNAT|SNAT|MASQUERADE|REDIRECT...]
- firewall-cmd --permanent --direct --add-rule [ipv4/ipv6] [raw|manage|nat|filter] [PREROUTING|POSTROUTING|INPUT|OUTPUT|FORWARD] [permission level:0、1...]  -p [protocol] --dport [port]  -j [ACCEPT|DROP|REJECT|LOG|NOTRACK|DNAT|SNAT|MASQUERADE|REDIRECT...]
