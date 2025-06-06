# HackTheChat - Boilerplates

Repositorio con boilerplates para la hackathon HackTheChat, incluyendo:

## 🚀 Proyectos incluidos

### 1. Extension Boilerplate
- **Ubicación**: `/extension-boilerplate`
- **Propósito**: Extensión de Chrome/Brave para modificar WhatsApp Web
- **Puerto**: No requiere (extensión de navegador)

### 2. Baileys Starter
- **Ubicación**: `/baileys-starter`
- **Propósito**: Bot de WhatsApp con conexión QR
- **Puerto**: 8081

## 📦 Configuración en servidor Ubuntu

### Prerrequisitos
```bash
# Actualizar sistema
sudo apt update && sudo apt upgrade -y

# Instalar Node.js 20 LTS
curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash -
sudo apt-get install -y nodejs

# Instalar PM2 para manejar procesos
sudo npm install -g pm2
```

### Instalación
```bash
# Clonar repositorio
git clone https://github.com/TU-USUARIO/hackthechat-boilerplates.git
cd hackthechat-boilerplates

# Configurar Baileys
cd baileys-starter
npm install

# Crear archivo .env
cp .env.example .env
# Editar .env con tus configuraciones

# Iniciar con PM2
pm2 start npm --name "hackthechat-bot" -- run dev
pm2 save
pm2 startup
```

### Acceso
- **Dashboard**: http://TU-IP-SERVIDOR:8081
- **QR Code**: http://TU-IP-SERVIDOR:8081/qr
- **Login**: http://TU-IP-SERVIDOR:8081/login (test/test)

## 🛠️ Desarrollo local

Ver instrucciones detalladas en commits anteriores.