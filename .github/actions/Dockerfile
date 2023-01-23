# Use a Python image as the base image
FROM python:3.11-slim-buster

# Copy the requirements file
COPY ./requirements.txt .

# update image and install curl
RUN apt update && apt add curl -y

# Install the Python dependencies
RUN pip install -r requirements.txt

ENV PATH="/usr/local/bin:$PATH"