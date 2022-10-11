FROM python:3.9

WORKDIR /code

COPY ./requirements.txt /code/requirements.txt

RUN pip install --no-cache-dir --upgrade -r /code/requirements.txt
RUN python consumer.py

COPY ./inventory /code/inventory

CMD ["uvicorn", "inventory.main:app", "--port", "8000"]

