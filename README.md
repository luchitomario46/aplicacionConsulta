# 📱 Aplicación de Consulta de Stock Interna

![React Native](https://img.shields.io/badge/React_Native-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![Expo](https://img.shields.io/badge/Expo-000020?style=for-the-badge&logo=expo&logoColor=white)

Aplicación móvil interna para consultar stock y precios en tiendas físicas.

## 🌟 Características Principales
- Autenticación JWT para empleados
- Consulta en tiempo real de stock por tienda
- Escáner de código de barras integrado
- Funcionalidad offline con caché local
- Panel administrativo Django para gestión

## 🚀 Primeros Pasos

### Prerrequisitos
- Node.js v18+
- Python 3.10+
- Expo CLI (`npm install -g expo-cli`)
- PostgreSQL (recomendado para producción)

### 🛠️ Instalación

#### Backend (Django)
```bash
# Clonar repositorio
git clone https://github.com/luchitomario46/aplicacionConsulta.git
cd aplicacionConsulta/backend

# Configurar entorno virtual
python -m venv venv
source venv/bin/activate  # Linux/Mac
# venv\Scripts\activate  # Windows

# Instalar dependencias
pip install -r requirements.txt

# Configurar variables de entorno
cp .env.example .env
# Editar .env con tus credenciales

# Migraciones iniciales
python manage.py migrate
python manage.py createsuperuser

# Iniciar servidor
python manage.py runserver
