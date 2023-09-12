FROM python:3.8

# Set the working directory
WORKDIR /usr/src/app

# Install system dependencies (only necessary ones)
RUN apt-get update && apt-get clean -y && rm -rf /var/lib/apt/lists/*

# Copy the requirements file into the container
COPY requirements.txt .

# Install pip and Jupyter dependencies
RUN pip install --no-cache-dir -r requirements.txt jupyter

# Copy the contents of the current directory to the container
COPY . .

# Command to run Jupyter Notebook on container startup
CMD ["jupyter", "notebook", "--ip=0.0.0.0", "--port=8888", "--no-browser", "--allow-root"]
