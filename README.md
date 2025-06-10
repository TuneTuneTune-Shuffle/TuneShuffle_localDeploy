# 🎵 TuneShuffle - Despliegue Docker

Este repositorio contiene la configuración necesaria para desplegar el sistema completo de **TuneShuffle** con:

- 🎧 **Frontend**: Next.js  
- ⚙️ **Backend**: FastAPI  
- 🛢️ **Base de datos**: MongoDB

Todo se ejecuta fácilmente usando **Docker** y **Docker Compose**.

---

## 📦 Requisitos

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)
- [Git](https://git-scm.com/)

---

## 🚀 Instalación y ejecución

### 1. Clonar el repositorio (con submódulos)

```bash
git clone --recurse-submodules https://github.com/TuneTuneTune-Shuffle/TuneShuffle_localDeploy.git
cd TuneShuffle_localDeploy
```

Si ya lo clonaste sin --recurse-submodules, ejecuta:

```bash
git submodule update --init --recursive
```

2. Construir y correr los contenedores
```bash
docker-compose up --build
```

Esto levantará los siguientes servicios:

🎧 Frontend: http://localhost:3000

⚙️ Backend API: http://localhost:8000

🛢️ MongoDB: mongodb://localhost:27017

📁 Estructura del proyecto
```bash
TuneShuffle_localDeploy/
├── docker-compose.yml           # Configuración de servicios
├── FrontEnd/                    # Submódulo con el cliente (Next.js)
└── Backend/                     # Submódulo con el servidor (FastAPI)
```

🧼 Detener los contenedores
Presiona Ctrl + C en la terminal o ejecuta:

```bash
docker-compose down
```
