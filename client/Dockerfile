FROM python:3.10-slim

WORKDIR /app

#RUN apt install

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    gcc \
    python3-dev && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*


COPY requirements.txt .
RUN pip install -r requirements.txt

COPY run_client.py .

CMD ["python3", "run_client.py"]
# ###
#
# 다음 주석을 지우고 docker 파일을 완성하자.
#
# ###