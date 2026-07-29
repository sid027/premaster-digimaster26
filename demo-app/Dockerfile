# Start from an official image that already contains Python
FROM python:3.12-slim

# Work inside the folder /app in the container
WORKDIR /app

# Copy the ingredient list and install the ingredients
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of our code into the container
COPY . .

# The app listens on port 5000 inside the container
EXPOSE 5000

# This command starts the app when the container starts
CMD ["python", "app.py"]
