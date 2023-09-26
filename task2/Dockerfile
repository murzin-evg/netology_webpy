FROM python:3.10

WORKDIR /webpy/

RUN git clone https://github.com/murzin-evg/netology_django

COPY settings.py /webpy/netology_django/3.2-crud/stocks_products/stocks_products/settings.py

RUN python3 -m pip install --no-cache-dir --no-warn-script-location --upgrade pip
RUN python3 -m pip install --no-cache-dir --no-warn-script-location --user -r /webpy/netology_django/3.2-crud/stocks_products/requirements.txt

RUN python3 /webpy//netology_django/3.2-crud/stocks_products/manage.py migrate

EXPOSE 80

CMD ["python3", "/webpy/netology_django/3.2-crud/stocks_products/manage.py", "runserver", "0.0.0.0:80"]
