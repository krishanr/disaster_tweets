# ============================== BASE ==========================================
FROM nvcr.io/nvidia/tensorflow:20.08-tf2-py3

RUN apt-get update

# Keeps Python from generating .pyc files in the container
ENV PYTHONDONTWRITEBYTECODE 1

# Turns off buffering for easier container logging
ENV PYTHONUNBUFFERED 1

WORKDIR /app
COPY . .

RUN pip install --upgrade pip
RUN python -m pip install -r requirements.txt