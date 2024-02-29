FROM python:latest

# Install Git
RUN apt-get update && apt-get install -y git

# Create directory for the project
RUN mkdir /build
WORKDIR /build

# Clone the repository
RUN cd /build && git clone https://github.com/Georgeclark04/dockertest.git
RUN pip3 install flask
RUN cd /build/dockertest/pyth

# Expose port
EXPOSE 8080

# Set entrypoint
ENTRYPOINT ["/build/dockertest/pyth/app.py"]
