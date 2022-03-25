# Reglas de iptables

> **INPUT** Configura las reglas de paquetes entrantes

> **FORWARD** Configura las reglas de reenvío de paquetes

> **OUTPUT** Configura las reglas de paquetes salientes

> **ACCEPT** Significa que el paquete podrá pasar.

> **DROP** Significa que no se permitirá que el paquete pase.

> **RETURN** Significa omitir la cadena actual y volver a la siguiente regla de la cadena en la que fue llamado.

**Borrar todas las reglas**
```
iptables -F
```

**Cambia la politica de entrada por defecto a rechazar**
```
iptables -P INPUT DROP
```

**Cambia la regla de entrada (-A INPUT) para aceptar (-j ACCEPT) paquetes tcp (-p tcp) de cualquier origen (-s 0/0) a cualquier destino (-d 0/0) en el puerto 22 (--dport 22)**
```
iptables -A INPUT -p tcp -s 0/0 -d 0/0 --dport 22 -j ACCEPT
```

