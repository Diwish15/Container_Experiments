# Use a base Python image
FROM python:3.9-slim
# Set environment variables to prevent Python from writing .pyc files and to ensure output is sent straight to terminal (unbuffered)

# Set the working directory inside the container
WORKDIR /app

# Copy the application code into the container
COPY app.py .

# Install necessary dependencies (if any)
# RUN pip install <dependencies>

# Run the Python application
CMD ["python", "app.py"]