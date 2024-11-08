FROM python:3.13

WORKDIR /scrapper

COPY . .

RUN pip install --no-cache-dir --upgrade pip \
    && pip install --no-cache-dir playwright==1.48.0 \
    && playwright install --with-deps

CMD ["python", "main.py"]