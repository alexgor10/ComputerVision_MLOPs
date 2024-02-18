FROM python:3.10

# Establece el directorio de trabajo dentro del contenedor en /app.
WORKDIR /app


COPY . .

# Instala dependencias
RUN pip install -r requirements.txt

# Establece un comando predeterminado para ejecutar el contenedor
CMD ["uvicorn", "app:app", "--host", "0.0.0.0", "--port", "8000"]