FROM python:3.9

WORKDIR /code

COPY ./requirements.txt .

RUN pip install --no-cache-dir --upgrade -r /code/requirements.txt

COPY . .

EXPOSE 10086
EXPOSE 8001
EXPOSE 443
EXPOSE 8000
EXPOSE 80

CMD ["uvicorn", "main:app", "--reload", "--port", "8001"]

