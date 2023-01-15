FROM python:3.8-slim-buster
COPY requirements.txt requirements.txt
RUN pip3 install -r requirements.txt
COPY . .
COPY ../hmse_job_utils ./hmse_job_utils
CMD ["python3", "transfer_weather_data.py"]