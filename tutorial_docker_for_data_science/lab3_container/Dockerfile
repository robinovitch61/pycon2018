# Specify base image
FROM python:3.6.5-slim

# Set up working directory
WORKDIR /app
COPY . /app

# Install dependancies
RUN pip --no-cache-dir install numpy pandas seaborn sklearn jupyter

# Set up port forwarding, exposing this port to world outside container
EXPOSE 8888

# Start jupyter on startup
CMD ["jupyter", "notebook", "--ip='*'", "--port=8888", "--no-browser", "--allow-root"]
