FROM python:3.9
WORKDIR /app
COPY requirements.txt .
RUN pip install -r /app/requirements.txt --no-cache-dir
# Скопировать всё необходимое содержимое 
# той директории локального компьютера, где сохранён Dockerfile,
# в текущую рабочую директорию образа — /app.
COPY . .
CMD ["python", "manage.py", "runserver", "0:8000"] 
