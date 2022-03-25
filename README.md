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


