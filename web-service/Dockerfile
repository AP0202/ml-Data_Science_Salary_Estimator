FROM python:3.7-slim

RUN pip install -U pip
RUN pip install pipenv 

WORKDIR /app

# COPY [ "Pipfile", "Pipfile.lock", "./" ]

# RUN pipenv install --system --deploy
COPY requirements.txt /tmp
RUN pip install --requirement /tmp/requirements.txt
# COPY . /app/tmp/

COPY [ "predict.py", "model_file.p","data_input.py", "./" ]

EXPOSE 9696

ENTRYPOINT [ "waitress-serve", "--listen=0.0.0.0:9696", "predict:app" ]