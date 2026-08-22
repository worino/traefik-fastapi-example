FROM python:3.12-slim

WORKDIR /app

COPY requirements.txt .

RUN pip install --no-cache-dir --upgrade -r requirements.txt

COPY . .

EXPOSE 80

CMD ["fastapi", "run", "app.py", "--port", "80", "--host", "0.0.0.0", "--proxy-headers"]