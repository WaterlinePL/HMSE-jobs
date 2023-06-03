FROM python:3.8-slim-buster
COPY hmse_hydrological_models/requirements.txt requirements.txt
RUN pip3 install -r requirements.txt
COPY hmse_hydrological_models hmse_hydrological_models
CMD ["python3", "./hmse_hydrological_models/main_cli.py"]