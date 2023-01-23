# Use a Python image as the base image
FROM python:3.11-slim-buster

# Copy the requirements file
COPY ./requirements.txt .

# update image and install curl
RUN apk update && apk add --no-cache curl -y

# Install the Python dependencies
RUN pip install --no-cache-dir -r requirements.txt

ENV PATH="/usr/local/bin:$PATH"