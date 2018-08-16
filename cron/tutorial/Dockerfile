FROM ubuntu:latest

RUN mkdir code

# Set the working directory to /app
WORKDIR /code

# Copy the current directory contents into the container at /app
COPY . /code

RUN apt-get update && apt-get install -y python3-pip cron && apt-get update

# Install any needed packages specified in requirements.txt
# RUN pip install --upgrade pip
RUN pip3 install -r requirements.txt
