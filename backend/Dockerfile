# backend/Dockerfile

FROM python:3.11-slim

# Establece el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copia los archivos de requirements.txt al contenedor
COPY requirements.txt .

# Instala las dependencias de Python
RUN pip install --no-cache-dir -r requirements.txt

# Copia el resto del código fuente al contenedor
COPY . .

# Comando por defecto
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
