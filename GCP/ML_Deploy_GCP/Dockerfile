FROM gcr.io/google.com/cloudsdktool/google-cloud-cli:455.0.0-slim

# Habilita logs en consola
ENV PYTHONUNBUFFERED True

# Establece el directorio de trabajo dentro del contenedor en /app.
WORKDIR /app
COPY . .

# Instala dependencias
RUN pip install -r requirements.txt

# Establece un comando predeterminado para ejecutar el contenedor
CMD ["uvicorn", "app:app", "--host", "0.0.0.0", "--port", "8080"]