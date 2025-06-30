FROM python:3.10-slim

COPY requirements.txt .
COPY main.py .

RUN pip install -r requirements.txt

CMD ["fastapi", "run", "main.py"]
