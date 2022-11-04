#FROM python:3.8-slim-bullseye
FROM python:3.8
WORKDIR /opt/api
COPY . .
RUN pip install --upgrade pip && pip install -r requirements.txt && python manage.py migrate
CMD ["python", "manage.py", "runserver"]
EXPOSE 8000
