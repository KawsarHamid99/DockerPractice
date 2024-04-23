FROM python:3.12


# Set environment variables for Python
ENV PYTHONUNBUFFERED 1


WORKDIR /django

COPY requirements.txt /django/

RUN pip install -r requirements.txt

COPY . /django/

CMD [ "python" , "manage.py" ,"runserver", "0.0.0.0:8000" ]