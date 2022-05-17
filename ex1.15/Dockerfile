FROM python:3.9
WORKDIR /usr/src/app
COPY . .
RUN pip install poetry
RUN poetry install
RUN apt-get update -y
RUN apt-get install fluidsynth -y
CMD poetry run invoke start ; bash