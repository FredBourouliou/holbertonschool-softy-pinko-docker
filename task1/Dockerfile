FROM ubuntu:latest

# Update APT
RUN apt-get update

# Upgrade currently installed software
RUN apt-get upgrade -y

# Install Python3 and pip3
RUN apt-get install -y python3 python3-pip

# Install Flask using pip3
RUN pip3 install flask

# Set up the working directory
WORKDIR /app

# Copy the application file
COPY ./api.py /app/api.py

# Run the Flask application
CMD ["python3", "/app/api.py"] 