# Reglas de iptables

**Acepte las entradas tcp de todas las redes al puerto 22**
```
iptables -A INPUT -p tcp -s 0/0 -d 0/0 --dport 22 -j ACCEPT
```

