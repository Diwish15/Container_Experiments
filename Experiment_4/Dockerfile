# Use Python as base image
FROM python:3.9-slim
# Set environment variables to prevent Python from writing .pyc files and to ensure output is sent straight to terminal (unbuffered)

# Set working directory
WORKDIR /app

# Copy application files
COPY . .

# Install dependencies
RUN pip install --no-cache-dir streamlit psycopg2

# Expose Streamlit port
EXPOSE 8501

# Run Streamlit
CMD ["streamlit", "run", "stream.py", "--server.port=8501", "--server.address=0.0.0.0"]