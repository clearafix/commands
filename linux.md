#Linux

###Disk usage

```
du -sh *
df -h
du -x /var/log/ | sort -n | tail -40
```

###Network tools

```
telnet localcost 25
dig example.com +trace
traceroute
curl
```
Start netcat server that returns HTTP response

```
while true; do echo -e "HTTP/1.1 200 OK\n\n $(date)" | nc -l localhost 8080; done
```
Start simple TCP netcat server that returns input from a command line:
```
nc -lk localhost 8080
```